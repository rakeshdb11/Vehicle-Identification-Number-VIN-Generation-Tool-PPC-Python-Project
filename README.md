# Vehicle-Identification-Number-VIN-Generation-Tool-PPC-Python-Project

**Description** This project develops a Python-based VIN generation tool for automobile industry. A Vehicle Identification Number (VIN) is a globally recognized code that uniquely identifies each vehicle. For automobile industry, VINs are critical for manufacturing records, regulatory compliance, warranty tracking, and fleet management.
The tool ensures VINs are generated according to the given model and Variant wise structure.

**Terminology used in Project:-**
1) MODEL_NAME --> It Represents the Model Name that is Used for Product Selling in Market.
2) MODEL_CODE --> It Represents the system code of that particular model that is used for Company internal Purposes and system transactions.(Production planning/ tracking & Inventory Controlling).
3) CHECK DIGIT --> The check digit in a Vehicle Identification Number (VIN) is the character, used as a mathematical safeguard to verify that the VIN is valid and not mistyped or altered. It helps detect errors in transcription and ensures the authenticity of the VIN.
4)  START_SERIAL_NO --> It represents the starting serial number structure of that particular model or variant.
5)  JOB_CODE --> When manufacturers generate VINs, they often include internal codes that represent specific details about the vehicle. One of these is referred to as a Job Code.
   - A Job Code is an internal production or assembly code used by manufacturers to identify a particular build, order, or 
    job during the manufacturing process.

    Pupose:-
    - Links the VIN to a specific production job/order in the factory.
    - Helps track manufacturing batches and assembly line details.
    - Ensures traceability for quality control, warranty claims, and recalls
6) PREFIX --> In the context of a Vehicle Identification Number (VIN), the term “prefix” usually refers to the starting characters of the VIN, that will same for EVery VIN of that particular Model.
7) MONTH_CODE --> It represents the Month in which Vehicle VIN is Created, Sometimes this code will vary model to model.
   same month has different month_code for different models, you have to maintain month code of all models.
8) YEAR_CODE -->  It represents the Year in which Vehicle VIN is Created, Sometimes this code will vary model to model.
   same Year has different Year_code for different models, you have to maintain Year code of all models.

**Overview:-**

1) Two Excel Workbooks are attached with this Project.

   a) MODEL_INFORMATION --> This sheet consists the all model wise data related to VIN Structures. This workbook has 7 different sheets, every sheets are serving different 
      purposes. (Do not change name of any sheet.)
      ~ Sheet1 (CHESIS_NO) :- Output of above project that is Vehicle Identification number will show in this sheet as per below Format.
   
     <img width="394" height="59" alt="image" src="https://github.com/user-attachments/assets/93e986f9-2d26-40ab-ac30-4ddb7c62bdb3" />
     
      Here,
   
      Date --> It represents for which date you have released the sequence.
   
      Prod_Seq --> It represents the Production sequence number in that month.
   
      Job_No --> It represents internal job ID that is allocated to particular VIN for internal tracking.
   
      Model --> It represents the Model code.
   
      Serial_No. --> It represents the Vehicle Identification Number.

      ~ Sheet2(SEQ) --> In this sheet you have to input the sequence 
   
   b) VIN_CREATION_HISTORY --> This sheet maintains the Past VIN Creation history with their time stamp.


   
   




