# EX-05-Feature-Generation


# AIM
To read the given data and perform Feature Generation process and save the data to a file. 

# Explanation

Feature Generation (also known as feature construction, feature extraction or feature engineering) is the process of transforming features into new features that better relate to the target.
 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature Generation techniques to all the feature of the data set
### STEP 4
Save the data to the file


# CODE:

# Data set:

# Ordinal Encoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("data.csv")

from sklearn.preprocessing import LabelEncoder,OrdinalEncoder

classes = ['Cold','Warm','Hot','Very Hot']

enc = OrdinalEncoder(categories = [classes])

enc.fit_transform(df[["Ord_1"]])

df['ord_1']=enc.fit_transform(df[["Ord_1"]])

df

# Label Encoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("data.csv")

from sklearn.preprocessing import LabelEncoder,OrdinalEncoder

classes = [0,1]

enc = OrdinalEncoder(categories = [classes])

enc.fit_transform(df[["Target"]])

df['target']=enc.fit_transform(df[["Target"]])

df

# Binary Encoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("data.csv")

!pip install category_encoders

from category_encoders import BinaryEncoder

be=BinaryEncoder()

newdata=be.fit_transform(df['bin_1'])

df1=pd.concat([df,newdata],axis=1)

df1

# OneHotEncoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("data.csv")

from sklearn.preprocessing import OneHotEncoder

ohe = OneHotEncoder(sparse=False)

df1 = df.copy()

enc = pd.DataFrame(ohe.fit_transform(df1[['City']]))

df1 = pd.concat([df1,enc],axis=1)

df1

# Encoding Data Set:

# Ordinal Encoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("Encoding Data.csv")

from sklearn.preprocessing import LabelEncoder,OrdinalEncoder

classes = ['Red','Blue','Green']

enc = OrdinalEncoder(categories = [classes])

enc.fit_transform(df[["nom_0"]])

df['Nom_0']=enc.fit_transform(df[["nom_0"]])

df

# Binary Encoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("Encoding Data.csv")

!pip install category_encoders

from category_encoders import BinaryEncoder

be=BinaryEncoder()

newdata=be.fit_transform(df['bin_1'])

df1=pd.concat([df,newdata],axis=1)

df1

# Titanic Data Set:

# Ordinal Encoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("titanic_dataset.csv")

from sklearn.preprocessing import LabelEncoder,OrdinalEncoder

classes = [1,2,3]

enc = OrdinalEncoder(categories = [classes])

enc.fit_transform(df[["Pclass"]])

df['ord_2']=enc.fit_transform(df[["Pclass"]])

df

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("titanic_dataset.csv")

from sklearn.preprocessing import LabelEncoder,OrdinalEncoder

classes = ['C','Q','S',np.nan]

enc = OrdinalEncoder(categories = [classes])

enc.fit_transform(df[["Embarked"]])

df['ord']=enc.fit_transform(df[["Embarked"]])

df

# Label Encoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("titanic_dataset.csv")

from sklearn.preprocessing import LabelEncoder,OrdinalEncoder

le = LabelEncoder()

df['Name1']=le.fit_transform(df['Name'])

df

# Binary Encoder:

import pandas as pd

import numpy as np

import seaborn as sns

from google.colab import files

uploaded = files.upload()

df = pd.read_csv("titanic_dataset.csv")

!pip install category_encoders

from category_encoders import BinaryEncoder

be=BinaryEncoder()

newdata=be.fit_transform(df['Sex'])

df1=pd.concat([df,newdata],axis=1)

df1

# OUTPUT:

# Data set:

# Ordinal Encoder:

![Screenshot (124)](https://user-images.githubusercontent.com/128019999/232314882-e8659f6a-6cb9-410e-a9ef-8bfb0751923e.png)
# Label Encoder:
![Screenshot (125)](https://user-images.githubusercontent.com/128019999/232314912-6eb6d519-31bd-4e5c-9e0a-687a63dc150d.png)
# Binary Encoder:
![Screenshot (126)](https://user-images.githubusercontent.com/128019999/232314935-65cab0f6-25df-4331-8a78-fc8bc06d0ffd.png)
# OneHotEncoder:

![Screenshot (127)](https://user-images.githubusercontent.com/128019999/232314952-245be8c4-f437-45e5-847d-755b6586cbb7.png)
# Encoding data set:

# Ordinal Encoder:

![Screenshot (128)](https://user-images.githubusercontent.com/128019999/232314963-2664ffff-a5fa-4bbd-951d-904d02e60ccf.png)
# Binary Encoder:
![Screenshot (129)](https://user-images.githubusercontent.com/128019999/232314971-608fd9e4-5076-4800-9c68-27393500862a.png)
# Titanic Data set:

# Ordinal Encoder:

![Screenshot (130)](https://user-images.githubusercontent.com/128019999/232315000-241a25d8-bd97-4840-8cc6-bfad4226a135.png)
![Screenshot (131)](https://user-images.githubusercontent.com/128019999/232315007-87391a77-9152-401a-945d-898b3d087178.png)

# Label Encoder:
![Screenshot (132)](https://user-images.githubusercontent.com/128019999/232315019-b84df54f-9719-4de7-b156-817d494639f3.png)

# Binary Encoder:
![Screenshot (133)](https://user-images.githubusercontent.com/128019999/232315047-5fdb3fe2-b9f3-4c8e-9a37-1b12372bf905.png)

# RESULT:

Thus the Feature Generation for the given data set is executed and output was verified successfully

