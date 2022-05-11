# Video lens correction
This program computes a 2 parameter lens distortion model on a single image and 
correct the input image or video, furthermore it saves the computed model.\
The program produces the following outputs: \
  If a video sequence is processed:\
    (1) The collection of extrated frames from the input video ("_original_frames" 
        folder), and the corrected ones ("_corrected_frames" folder).\
    (2) An output file called "output.avi" with the corrected video sequence. \
  If a single image is processed:\
    (1) A png image with the output name finished in "_undistorted".\
    Regardless, a file with the .ldm extension is saved, which contains the lens distortion model.\

The libpng header and libraries are required on the system for compilation and execution. 
This program takes 11 parameters (one of them is optional):"exe_file input.png/input.avi output high_threshold_Canny initial_distortion_parameter final_distortion_parameter 
distance_point_line_max_hough angle_point_orientation_max_difference typo_of_lens_distortion_model center_optimization undistorted_image_magnification model_ldm"
