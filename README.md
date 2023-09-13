# BMT-synthetic-datasets
Synthetic datasets for the Burst and Memory-aware Transformer model.

Datasets contain two categories.
- 'data_exp_01': datasets of an exponential inter-event time distribution.
- 'data_power_02': datasets of a power-law inter-event time distribution with an exponent 2.1 to 2.9.

Each datasets contain below four files.
- train.pkl: train datasets
- dev.pkl: validation datasets
- test.pkl and test1.pkl: test datasets

The structure of 'pkl' file
- Dictionary with the keys of 'train', 'dev', 'test', 'test1', 'dim_process', and 'args'
  - 'dim_process' is 1 for the BMT model
- Each dictionary is the list of events with keys of 'time_since_start', 'time_since_last_event', and 'type_event'
  - 'type_event' is 0 for the BMT model
