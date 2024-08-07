### [επιστροφή στα περιεχόμενα](./README.md)


# Ανάλυση Δεδομένων με το Pandas

Η βιβλιοθήκη [Pandas](https://pandas.pydata.org) παρέχει συναρτήσεις για την εύκολη ανάγνωση δεδομένων από αρχεία (π.χ. excel, csv) και τον χειρισμό αυτών.

Μια σύνοψη των δυνατοτήτων του Pandas μπορεί να βρέθει στον παρακάτω σύνδεσμο:
https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf 


# Δημιουργία Dataframe
```python
# Φόρτωση της βιβλιοθήκης Pandas
import pandas as pd

# Εισαγωγή δεδομένων σε λίστα
data = {'Όνομα': ['Μανώλης', 'Κώστας', 'Ελένη', 'Δήμητρα'], 
        'Ηλικία': [20, 21, 19, 22], 
        'BMI': [24, 28, 25, 22]}  
  
# Create DataFrame  
df = pd.DataFrame(data)  

df
```



# Διάβασμα δεδομένων από αρχείο excel ή csv

Για την εύκολη επεξεργασία των δεδομένων ενός πίνακα του excel ή ενός αρχείου csv, μπορείτε να δημιουργήσετε με αυτά ένα dataframe με χρήση της κατάλληλης εντολής.

```python
from google.colab import drive
drive.mount('/content/drive')
```

```python
# Φόρτωση κατάλληλων βιβλιοθηκών
import pandas as pd

url="/content/drive/MyDrive/Colab Notebooks/2450_Efarmoges_Pliroforikis/data/pelatologio.xlsx"

# Διάβασμα αρχείου excel σαν dataframe
df = pd.read_excel(url)

df.head()
```

# Συναρτήσεις του Pandas

**`head`**

Η συνάρτηση `head()` στα Pandas μπορεί να χρησιμοποιηθεί για την εμφάνιση δείγματος δεδομένων που υπάρχουν στο DataFrame

```python
# Εμφάνιση δείγματος του dataframe
df.head()
```

```python
# Εμφάνιση όλων των ονομάτων των παραμέτρων
df.columns
```

```python
# Δημιουργία λίστας με της επικεφαλίδες κάθε στήλης
epikefalides = df.columns.values.tolist()
print(epikefalides)
```

```python
# Εμφάνιση των τιμών μιας στήλης
df["BMI"]
```

```python
# Εμφάνιση της τιμής μιας στήλης σε μια συγκεκριμένη γραμμή
df["BMI"][2]
```

```python
# Προσθήκη στήλης
df["Height_cm"] = df["Height"]*100.0

df
```

```python
# Αριθμός εμφάνισεων των διαφορετικών τιμών μιας στήλης
df["PhysicalActivityPerWeek"].value_counts()
```

```python
# Βασική στατιστική ανάλυση ανά στήλη
df.describe()
```

```python
# Μέση τιμή για συγκεκριμένη στήλη (υποδηλώνεται από το  axis=0)
mean_height = df["Height"].mean(axis=0)
print(mean_height)
```

```python
min_BMI = df["BMI"].min(axis=0)
print(min_BMI)
```

```python
# Βαθμός συσχέτισης των στηλών ανα δυάδες
df.corr()
```

```python
# Ταξινόμηση ανα συγκεκριμένη στήλη
df.sort_values(by="BMI")
```

"""# 4.&nbsp;Εύρεση δεδομένων με κριτήρια (query)



"""

# Εύρεση του πελάτη με το επίθετο "Clark"
df.query("LastName == 'Clark'")

# Εύρεση του πελάτη με το επίθετο "Clark" και γένους αρσενικού
df.query("LastName == 'Clark' and Gender =='Male'")

# Εύρεση πελατών με έτος γέννησης μεγαλύτερου του 2002
df.query("YearOfBirth > 2002")

# Εύρεση πελατών με έτος γέννησης μεγαλύτερου του 2002 με δυσανεξία στη λακτόζη
df.query("YearOfBirth > 2002 and LactoseIntorelant == True")

# Askisi
df1 = df.query("YearOfBirth < 1995 and Height > 1.80 and PhysicalActivityPerWeek == 1 and LactoseIntorelant == True")
df1

df1.describe()

"""# 5.&nbsp;Γραφικές παραστάσεις με το Pandas

Το pandas παρέχει ευκολία όχι μόνο στην γραφική απεικόνιση των δεδομένων ενός dataframe αλλά και στην γραφική απεικόνιση ποικίλων αναλύσεων των δεδομένων αυτών

## Scatter (x-y) plot

Με χρήση της εντολής `plot.scatter()` μπορούμε να απεικονίσουμε σε διάγραμμα x-y όποιες από τις 2 στήλες του dataframe θέλουμε.
"""

df.corr()

df.plot.scatter("BMI", "Height")

# Το ίδιο γράφημα μπορεί να δημιουργήθεί και με την βιβλιοθήκη matplotlib
import matplotlib.pyplot as plt
plt.scatter(df["Weight"], df["Height"])
plt.show()

"""### Άσκηση
Δημιουργήστε σε ένα κελί το x-y διάγραμμα των στηλών Weight και ΒΜΙ

## Ιστογράμματα (histograms)
Για να υπολογίσουμε την κατανομή των δεδομένων μια στήλης μπορούμε να χρησιμοποιήσουμε την εντολή `hist()`.
"""

df.hist("Weight", bins=5)

"""#### Άσκηση
Δημιουργήστε ένα ιστόγραμμα για την στήλη Height και με αριθμό bins 10.

## Boxplots (Θηκόγραμμα)

Τα [boxplots](https://en.wikipedia.org/wiki/Box_plot#/media/File:Boxplot_vs_PDF.svg) είναι ένας βολικός τρόπος γραφικής απεικόνισης πέντε αριθμητικών δεδομένων μιας σειράς παρατηρήσεων: της μικρότερης
παρατήρησης του πρώτου τεταρτημόριου (Q1), της διαμέσου (δ) του τρίτου τεταρτημόριου (Q3), και της μεγαλύτερης παρατήρησης.

Με το Pandas μπορούμε δημιουργήσουμε για οποιαδήποτε στήλη θέλουμε με την εντόλη `boxplot()`.
"""

df.boxplot(column=["BMI", "Weight"])

"""### Άσκηση
Δημιουργήστε ένα boxplot για την παράμετρο του υψους σε εκατοστά (Height_cm)
"""

df.boxplot(column=["Height_cm"])

"""## Scatter Matrix plots

Η συγκεκριμένη κατηγορία γραφημάτων βοηθά να έχουμε μια συνολική εικόνα για το dataframe σχετικά με την κατανομή των δεδομένων αλλά και μια γραφική απεικόνιση της συσχέτισης τους ανά δυάδες.

Στο pandas δημιουργούνται με την εντολή `plotting.scatter_matrix()`
"""

# Αφαίρεση των στηλών από το dataframe που δεν είναι integer ή real
df = df.drop(columns=["FirstName", "LastName", "Gender", 'LactoseIntorelant', 'Diabetic'])
df

# Δημιουργία του γραφήματος
pd.plotting.scatter_matrix(df)

# Αύξηση του μεγέθους της εικόνας
pd.plotting.scatter_matrix(df, figsize=(15,15))

"""# 6.&nbsp;Δημιουργία Reports

Με χρήση της κατάλληλης βιβλιοθήκης είναι εφικτό να δημιουργηθεί με αυτοματοποιημένο τρόπο ένα report με την συνολική ανάλυση των δεδομένων ενός dataframe.
"""

#εγκατασταση βιβλιοθήκης
!pip install sweetviz

# importing sweetviz
import sweetviz as sv

#analyzing the dataset
my_report = sv.analyze(df)

#display the report
my_report.show_notebook()

#analyzing the dataset against a target variable
my_report = sv.analyze(df, target_feat="Weight")

#display the report
my_report.show_notebook()

"""# 7.&nbsp; Διαβάσμα δεδομένων από σελίδες της Wikipedia

Η βιβλιοθήκη Pandas έχει την δυνατότητα να διαβάζει δεδομένα κατευθείαν από πίνακες που υπάρχουν σε σελίδες της Wikipedia και άλλες ιστοσελίδες.

Η εντολή που πρέπει να χρησιμοποιηθεί είναι η `pd.read_html(url)`

Για παράδειγμα, έστω ότι θέλουμε να επεξεργαστούμε τα στοιχεία του πίνακα που βρίσκονται στον παρακάτω σύνδεσμο: 

https://en.wikipedia.org/wiki/List_of_sovereign_states_by_body_mass_index


Χρησιμοποιούμε τις παρακάτω εντόλες για να δημιουργήσουμε ένα dataframe από τα στοιχεία του πίνακα που εμπεριέχεται στην συγκεκριμένη ιστοσελίδα

Σημείωση: Είναι πιθανόν να δημιουργηθεί μια λίστα με τους διάφορους πίνακες που περιέχει η συγκεκριμένη ιστοσελίδα, οπότε θα χρειαστεί να επιλέξουμε την κατάλληλη.


"""

import pandas as pd
import numpy as np

# εδώ δηλώνετε την ιστοσελίδα που περιέχει των πίνακα με τα δεδομένα
url = "https://en.wikipedia.org/wiki/List_of_sovereign_states_by_body_mass_index"

# Διάβασμα των δεδομένων της ιστοσελίδας
#tables = pd.read_html(url)
tables = pd.read_html(url)

tables

# Αποθήκευση ως dataframe τα συγκεκριμένα στοιχεία της επιλογής σας.
df_bmi = tables[0]
df_bmi

# Ανάλυση των δεδομένων
df_bmi.describe()

# Για να μπορέσουμε να αναλύσουμε τα δεδομένα μας θα πρέπει να εξασφαλίσουμε ότι 
# - υπάρχουν διαθέσιμα στοιχεία για όλες τις χώρες
# - τα δεδομένα διαβάζονται με τον σωστό τύπο τους, π.χ. float και όχι string


# Για να κρατήσουμε μόνο τις γραμμές (χώρες) που υπάρχουν διαθέσιμα στοιχεία
# εκτελούμε την παρακάτω εντολή

df_bmi = df_bmi[df_bmi['Both'] != '—']
df_bmi

df_bmi.dtypes

# Για κάθε μια από τις στήλες του BMI ορίζουμε ότι τα δεδομένα είναι τύπου "float"
df_bmi['Both'] = df_bmi['Both'].astype(float)
df_bmi['Male'] = df_bmi['Male'].astype(float)
df_bmi['Female'] = df_bmi['Female'].astype(float)

df_bmi.dtypes

# επιτυχής ανάλυση των δεδομένων
df_bmi.describe()

"""## Άσκηση

Χρησιμοποιώντας τα στοιχεία του παραπάνω dataframe


Υπολογίστε τα παρακάτω:
* Τον παγκόσμιο μέσο όρο BMI των αντρών και των γυναικών
* Τον αριθμό των χωρών που έχουν ΒΜΙ αντρών 25-30 (κατηγορία overweight)
* Τον αριθμό των χωρών που έχουν BMI γυναικών κάτω από 18.5 (κατηγορία underweight)

"""

average_male = df_bmi["Male"].mean(axis=0)
average_female = df_bmi["Female"].mean(axis=0)
print("Το μέσο ΒΜΙ των ανδρών είναι", average_male)
print("Το μέσο ΒΜΙ των γυναικών είναι", average_female)

df_over = df_bmi.query("Male > 25 and Male < 30")
df_over.count()

df_under = df_bmi.query("Female < 18.5")
df_under.count()

"""# 8.&nbsp;Άσκηση

Χρησιμοποιήστε το αρχείο `nutrition.xlsx` που θα βρείτε στο eclass και υπολογίστε τα παρακάτω:

1. Αν υπάρχουν ποτά που να περιέχουν περισσότερες από 100 θερμίδες 
2. Αν υπάρχουν θαλασσινά που να περιέχουν πάνω από 20 γρ πρωτεινής
3. ποιες δυο μεταβλητές έχουν την μεγαλύτερη συσχέτιση (θετική ή αρνητική) και δημιουργήστε το αντίστοιχο x-y διάγραμμά τους
4. ποιες δυο μεταβλητές παρουσιάζουν την μικρότερη συσχέτιση και δημιουργήστε το αντίστοιχο x-y διάγραμμά τους

"""

# Φόρτωση κατάλληλων βιβλιοθηκών
import pandas as pd

url="/content/drive/MyDrive/Colab Notebooks/2450_Efarmoges_Pliroforikis/data/nutrition.xlsx"

# Διάβασμα αρχείου excel σαν dataframe
df = pd.read_excel(url)

df

df.query("Category == 'Drinks_Alcohol_Beverages' and Calories > 100")

df.query("Category == 'Fish_Seafood' and Protein > 20")

df["Category"].value_counts()

df.corr()

df.plot.scatter("Fat", "Sat_Fat")

df.plot.scatter("Fat", "Fiber")

df["Category"].value_counts()