# cut-car-parking-frames

This project is used to track and cut the frames that cars go into or go out the parking lots.

Firstly, run car_tracking.ipynb to track the cars in a video, or all videos in a folder, or a list of videos written in a text file. It is based on the github https://github.com/mikel-brostrom/Yolov5_DeepSort_OSNet.git that uses YOLOv5 to detect objects and deep sort to track those objects. The inputs are the videos that have the words 'extracted_videos' in their paths. The outputs are the videos and text files that have the paths are the input video paths replacing 'extracted_videos' by 'results'. These output videos show tracking all cars in those videos while these output text files present the numerical order and the coordinates of the cars, and the size of the frames. 

Secondly, run extract_subclip.ipynb to cut the frames that cars go into or go out the parking lots. The inputs are the text files from step one, while the outputs are the videos which only show the cars go into or go out the parking lots. The paths of these videos are the original video paths replacing 'extracted_videos' by 'results2'