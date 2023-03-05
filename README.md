# MetaEHR

This is the source code for MetaEHR, which is a Python package for few-shot clinical prediction problems, including time-associated prediction targets and time-independent prediction targets.

The time-associated algorithm is the implementation of our work **TAML**: **T**ime-**a**ssociated **M**eta **L**earning for Clinical Prediction. The time-independent algorithm can be any of following meta learning algorithm: MAML, ProtoNet.

# Features (What function does MetaEHR have?)
1. Problem type
  - Time-associated targets. For example, mortality time, ICU length of stay.
  - Time-independent targets. For example, AKI, pneumonia.
  
2. Input file type
  - Single file. For example, preoperative data, flowsheet data, time-series data.
  - Multifple files. For example, all of the above data types from the same patients.
  
3. Other required files
  - Outcome file, which serves as candidate for meta-tasks.
  - Predictive target file, which is the true few-shot target.
  - (Optional) Validation target, which will be randomly chose if not specified.
