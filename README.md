# SEED
SEED新能源赛道：电动汽车充电站充电需求预测

test: Data visualization and a single station prediction use a single-layer RNN model

baseline+geography+workday：Added the feature of whether the date is a working day



Tasks to be completed：

- reshape the input tensor like [500,364,15] to [500*344,14,15], set the batchsize = 344.  The setting of the batchsize can grant the order of the time series is correct in one batchsize . The model will correctly learn temporal features because different batches of learning are independent.
- Embeddings can be used to encode dates, and further, embeddings can be utilized to encode all features.
