sct_deepseg_lesion models
===============================================================================

This folder contains the sct_deepseg_lesion models:
    - t2_ax_lesion.h5 trained on a private dataset including 211 MR volumes
    - t2_lesion.h5 trained on a private dataset including 709 MR volumes
    - t2s_lesion.h5 trained on a private dataset including 416 MR volumes

    This dataset was created on 26 May 2018.

The data used for training the model can be found under: `duke/projects/ms_seg/seg_paper/data_ms`. Only data of MS patients (not healthy controls, HCs) were used for training and validation but the model was tested on both MS and HCs.

The dataset.pkl (found here: https://github.com/spinalcordtoolbox/deepseg_sc_models/tree/master/src/spinalcordtoolbox/data/deepseg/sc) contains the information on the subjects used, their pathology, train/val/test, etc that was used for training deepseg_sc. In order to compare other models with deepseg_lesion, pick out only MS patients (specified under the column patho) and split them according to the train/val/test split. This should give an exact comparison.
