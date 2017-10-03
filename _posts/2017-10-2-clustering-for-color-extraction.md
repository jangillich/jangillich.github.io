https://labs.tineye.com/color/

3D-Dbscan

from sklearn.cluster import DBSCAN
import numpy as np
data = np.random.rand(500,3)

db = DBSCAN(eps=0.12, min_samples=1).fit(data)
labels = db.labels_
from collections import Counter
Counter(labels)