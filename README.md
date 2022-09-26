# Virtual-Assistent-for-visually-impaired

The system is designed in such a way in which the blind person can take the help of An Application which inturn laptop based network system. It works on object detection using ssd_mobile.net algorithm and TENSORFLOW APIs . It has a core feature of approximate distance calculation and Voice - Based wireless feedack generation w.r.t the DISTANCE CALCULATION. It makes the work of Blind easy,efficient and reliable by sending wireless Voice based feedback whether the particular object is either too close to him or is it at a safer distance. The same system can be used from Obstacle Detection. 

STEPS:
1. TensorFlow Installation
A typical user can simply install it on Anaconda Prompt with following commands.

#for cpu:

  pip install tensorflow
  
#for gpu:

  pip install tensorflow-gpu

2.Now you need to download the TensorFlow model repository from
 
git clone https://github.com/tensorflow/models.git

3.PROTOBUF COMPILATION

Next you have to Convert the .protos file to .py file extensions.

This can be done via Protobuf Compilation. For achieving this we we’ll need Google Protobuf Releases. Head on to the link and Download the protobuf version which satisfies your system compatibility. I prefer win_64 which supports my system. After downloading and extracting it make sure to add it’s path in the environment variable otherwise it’ll still give you errors as ‘proto is not recognised as an internal or external batch file’. So,make sure it is done!

Further , inside of tensorflow/models/research/ directory :

Hit the following command:

#from tensorflow/models/research

protoc object_detection/protos/*.proto --python_out=.

Now it will successfully converted and executed.
