# TGNN/tgnn_model.ipynb

This file defines the full **data preparation and training pipeline** for graph-based learning using the model and demo dataset from Hu et al. (2024).

Each dataset sample corresponds to **one strain path**, where grains in a representative volume element (RVE) are modeled as nodes in a graph and trained to predict grain-scale responses over strain increments.

## Overview

The code provides functionality to:

- Construct **graph data objects** representing grain connectivity using demo_dataset_PN8_sq100.hdf5 and edge network (RVE24-n100_edge_feature.pickle)
- Create PyG 'DataLoader's for training and testing.
- Perform **model training and evaluation**

---

# experimental-data-gnn\create_pyg_graph.ipynb

This file defines the full **data processing** for graph-based learning using experimental grain neighbour, shear, orientation, size and phase data.

## Overview

The code provides functionality to:

- Extract **grain neighbour** data
- Normalise variables
- Construct **graph data objects**

---

# experimental-data-gnn\gnn_single_step.ipynb
This file defines the full **model training and evaluation pipeline** for graph-based learning using experimental grain neighbour, shear, orientation, size and phase data.

## Overview

The code provides functionality to:

- Create PyG 'DataLoader's for training and testing.
- Perform **model training and evaluation**
- 
---
