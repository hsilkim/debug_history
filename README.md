Issue 
>> tensorboard :  adds "tf.summary.scalar"

InvalidArgumentError (see above for traceback): You must feed a value for placeholder tensor 'data_1/target_words' with dtype int32 and shape [128,1]
 [[Node: data_1/target_words = Placeholder[dtype=DT_INT32, shape=[128,1], _device="/job:localhost/replica:0/task:0/device:CPU:0"]()]]
 
 Solution
 >> tf.reset_default_graph()
