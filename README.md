# FACE AND EYE DETECTION 
This is basically an implementation of a Face and Eye Detection using Opencv Default Haar Cascade .

#### Required Modules :
  - Numpy   
    ```bash
      pip install numpy
    ```
  - Opencv   
    ```bash
      pip install opencv-python
    ```
-->Haar Cascades can be used to detect any types of objects as long as you have the appropriate XML file for it. You can even create your own XML files from scratch to detect whatever type of object you want

-->cv2.CascadeClasifier() is created and required xml file is loaded in it

--> Afterwards the detection is done using the CascadeClasifier().detectMultiScale() method which returns the boundry rectangles of detect faces and eyes.

-->Syntax: cv2.putText(image, text, org, font, fontScale, color[, thickness[, lineType[, bottomLeftOrigin]]])

    Parameters:
    image: It is the image on which text is to be drawn.
    text: Text string to be drawn.
    org: It is the coordinates of the bottom-left corner of the text string in the image. The coordinates are represented as tuples of two values i.e. (X coordinate value, Y coordinate value).
    font: It denotes the font type. Some of font types are FONT_HERSHEY_SIMPLEX, FONT_HERSHEY_PLAIN, , etc.
    fontScale: Font scale factor that is multiplied by the font-specific base size.
    color: It is the color of text string to be drawn. For BGR, we pass a tuple. eg: (255, 0, 0) for blue color.
    thickness: It is the thickness of the line in px.
    lineType: This is an optional parameter.It gives the type of the line to be used.
    bottomLeftOrigin: This is an optional parameter. When it is true, the image data origin is at the bottom-left corner. Otherwise, it is at the top-left corner.

    Return Value: It returns an image.
    
-->Syntax: cv2.rectangle(image, start_point, end_point, color, thickness)

    Parameters:
    image: It is the image on which rectangle is to be drawn.
    start_point: It is the starting coordinates of rectangle. The coordinates are represented as tuples of two values i.e. (X coordinate value, Y coordinate value).
    end_point: It is the ending coordinates of rectangle. The coordinates are represented as tuples of two values i.e. (X coordinate value, Y coordinate value).
    color: It is the color of border line of rectangle to be drawn. For BGR, we pass a tuple. eg: (255, 0, 0) for blue color.
    thickness: It is the thickness of the rectangle border line in px. Thickness of -1 px will fill the rectangle shape by the specified color.

    Return Value: It returns an image.
    
-->Syntax: cv2.imshow(window_name, image)
    Parameters: 
    window_name: A string representing the name of the window in which image to be displayed. 
    image: It is the image that is to be displayed.
    Return Value: It doesn’t returns anything.
-->cap.release() stops the video capture
-->cv2.destroyAllWindows() close all windows