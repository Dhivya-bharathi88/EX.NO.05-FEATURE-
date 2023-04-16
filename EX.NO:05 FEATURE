import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("Encoding Data.csv")
print(df)

import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("Encoding Data.csv")
from sklearn.preprocessing import LabelEncoder,OrdinalEncoder
classes = ['Cold','Warm','Hot','Very Hot']
enc = OrdinalEncoder(categories = [classes])
enc.fit_transform(df[["ord_2"]])
df['Ord_2']=enc.fit_transform(df[["ord_2"]])
df

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

import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("Encoding Data.csv")
from sklearn.preprocessing import LabelEncoder,OrdinalEncoder
classes = ['N','Y']
enc = OrdinalEncoder(categories = [classes])
enc.fit_transform(df[["bin_2"]])
df['Bin_2']=enc.fit_transform(df[["bin_2"]])
df

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

import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("titanic_dataset.csv")
print(df)


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
classes = [0,1,2,3,4,5,6]
enc = OrdinalEncoder(categories = [classes])
enc.fit_transform(df[["Parch"]])
df['ord']=enc.fit_transform(df[["Parch"]])
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

import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("data.csv")
print(df)

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

import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("data.csv")
from sklearn.preprocessing import LabelEncoder,OrdinalEncoder
classes = ['High School','Diploma','Bachelors','Masters','PhD']
enc = OrdinalEncoder(categories = [classes])
enc.fit_transform(df[["Ord_2"]])
df['ord_2']=enc.fit_transform(df[["Ord_2"]])
df

import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("data.csv")
from sklearn.preprocessing import LabelEncoder,OrdinalEncoder
classes = ['N','Y']
enc = OrdinalEncoder(categories = [classes])
enc.fit_transform(df[["bin_2"]])
df['Bin_2']=enc.fit_transform(df[["bin_2"]])
df

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

import pandas as pd
import numpy as np
import seaborn as sns
from google.colab import files
uploaded = files.upload()
df = pd.read_csv("data.csv")
from sklearn.preprocessing import LabelEncoder,OrdinalEncoder
le = LabelEncoder()
df['city']=le.fit_transform(df['City'])
df

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
