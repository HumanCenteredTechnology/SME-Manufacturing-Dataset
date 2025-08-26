# Discrete Manufacturing Dataset

This repository contains the **discrete manufacturing dataset** presented in the paper:

> **Data-Driven Insights through Industrial Retrofitting: An Anonymized Dataset with Machine Learning Use Cases**  
> Available [here](https://www.mdpi.com/1424-8220/23/13/6078).

The dataset is provided freely for research and educational purposes. Please check the original paper for a complete description of the dataset and its statistics.

---

## 📂 Dataset Structure

- **`company_A.csv`**  
    ts: (string) a timestamp in the format YYYY-MM-DD HH:mm:ss+TZ,
    asset: (string) an identifier for the machine used;
    items: (int) the number of items produced in the time span;
    status: (int) the machine state where 0 is idle, 1 is manual production mode;
    2 is automatic production mode and 3 is an alarm or interrupted state;
    power_avg: (int) the average power consumed, in kilo-watts;
    cycle_time: (int) the total time, in seconds, to produce the items.
  
- **`company_A_labelled_subset.csv`**  
  ts: (string) a timestamp in the format YYYY-MM-DD HH:mm:ss+TZ;
  asset: (string) an identifier for the machine used;
  items: (int) the number of items produced in the time span;
  status: (int) the machine state where 0 is idle, 1 is manual production mode,
  2 is automatic production mode and 3 is an alarm or interrupted state;
  power_avg: (int) the average power consumed, in kilo-watts;
  cycle_time: (int) the total time, in seconds, to produce the items;
  product: (int) a product identifier ranging from 0 to 13.
  
- **`company_B.zipcompany_A_labelled_subset.csv`**  
  ts: (string) a timestamp in the format YYYY-MM-DD HH:mm:ss+TZ;
  asset: (string) an identifier for the machine used;
  status: (string) the machine state
  (Alarm, Standby, MachineOn, Production, Loading, Tooling);
  alarm_time: (int) the time spent in the alarm state;
  loading_time: (int) the time spent preparing the machine for production;
  tooling_time: (int) the time spent preparing machine tools;
  maintenance_time: (int) the time spent performing machine maintenance;
  support_time: (int) the time spent performing machine repair;
  power_avg: (int) the average power consumed, in kilo-watts;
  power_max: (int) the highest power consumption value in the 1-minute period;
  power_min: (int) the lowest power consumption value in the 1-minute period.


---

## 📖 Citation

If you use this dataset in your research, please cite the original publication:

```bibtex
@article{atzeni2023data,
  title={Data-driven insights through industrial retrofitting: An anonymized dataset with machine learning use cases},
  author={Atzeni, Daniele and Ramjattan, Reshawn and Figli{\`e}, Roberto and Baldi, Giacomo and Mazzei, Daniele},
  journal={Sensors},
  volume={23},
  number={13},
  pages={6078},
  year={2023},
  publisher={MDPI}
}
