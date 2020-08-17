# invoice-auto-fill

Computer Vision(Faster R-CNN) solution to extract necessary information from an invoice and fill required data. 
Training is done on Broadband bills of Indian Vendors namely Airtel and ACT (came out from Empathy research)
We can extend it to other operators like Hathway, Tatasky broadband and similar operators.

First - a Cusom Object Detection model has been used (Faster RCNN) to train on ~100 samples. The images have been resized
to 600x600 during Training to make it faster
Training is done on Cloud GPU.
The trained model with all artifacts - like the frozen_interface graph, the labelMap pbtxt file
have all been saved.

In the demo video - we will focus on the Prediction part. 
We will also see a typical Expense filling process in my.oracle.com and the pains associated with it.

The page shown in demo(while creating the Expense Item) where we fill all the details can be completely automated.
All these details can be fetched from the Invoice automatically with the help of Computer Vision.
We require the Name,Date,Amount and other details.The trained model can detect the portions of interest in the Broadband bill/invoice.
The corresponding boxes have been identified with a Faster RCNN custom model and the text extracted by OCR

Not only this - the verification of Expenses can also be automatically done without any human error/bias
We can extract the Employee name/phone/email if we want and do automated checks.

