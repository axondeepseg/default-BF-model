# model_seg_rat_axon-myelin_bf
Default Bright-Field (BF) optical microscopy model that works at a resolution of 0.1 micrometer per pixel.

# Steps to train this model
1. Get `ivadomed` version: [[83f11d4]](https://github.com/ivadomed/ivadomed/pull/980/commits/83f11d4433f8a8679d11bb7667a4e1d9e02c56b1)
2. Get the data: `data_axondeepseg_bf_training` (duke/projects/axondeepseg/20211105_bf_datasets/data_axondeepseg_bf_training)
3. Copy the "model_seg_rat_axon-myelin_bf_training.json" and "split_dataset.joblib" files, and update the following fields: `fname_split`, `path_output`, `path_data` and `gpu_ids`.
4. Run ivadomed: `ivadomed -c path/to/the/config/file`
5. The trained model file will be saved under the `path_output` directory.
