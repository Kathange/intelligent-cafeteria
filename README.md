# intelligent-cafeteria
This is a undergraduate project from Department of Computer Science and Information Engineering at Chang Gung University.

The project start in 2023/07 and end in 2024/12. We have four person in group, and our advisor is YP Chao.

Undergradurate Project : 剩食傳說 - 3D智助餐系統

# Project Introduction
 **Abstract**

Taiwan has entered an aging society, making balanced dietary intake for the elderly extremely important. Many long-term care institutions monitor the meals taken by the elderly to evaluate their nutritional intake. However, factors such as personal preferences, age-related chewing difficulties, and excessive portion sizes can lead to food waste, resulting in actual nutrient intake being lower than expected.

Our 3D Intelligent Cafeteria System consists of a depth camera, edge computing device, and card reader. Customers simply place their self-served trays on our rack and press the capture button. The system then takes a photo and captures depth information. The photo undergoes semantic segmentation to identify the types and positions of the food items. Subsequently, the depth at each identified position is integrated to determine the volume of each dish. By matching this data with the Ministry of Health and Welfare's food calorie database, the system can calculate the price, calories, and other nutritional components of each dish.

The required equipment for the system includes a depth camera (Intel RealSense L515), Nvidia Jetson Orin Nano, display screen, acrylic enclosure, Arduino RC522, ultrasonic sensors, RFID recognition, and LED light strips. The functionalities of the equipment are detailed below:

- **RFID Recognition:** When a customer places their card near the device, the RFID is read to verify membership status.
- **Line Official Account:** The customer's transaction records and nutritional information for each meal are sent to their Line account, allowing them to query past records at any time.
- **Ultrasonic Detection:** When a tray is placed into the system, a 5-second countdown begins. If the tray is continuously detected during the countdown, the system proceeds to capture an image.
- **Volume Calculation:** The depth information obtained by the depth camera is input into a pre-calculated regression equation to determine the volume.
- **Dish Recognition:** A self-trained U-net model performs semantic segmentation to identify the types of dishes.
- **Result Integration:** The identified dish types and calculated volumes are matched with data from a pre-established database, providing customers with detailed information.

This system is not only applicable within long-term care institutions but, due to its lightweight and edge computing capabilities, it can also be widely deployed in various restaurants. It offers users automated dietary recording functions, while businesses can analyze food waste to understand the relationship between dining demographics and leftover food.

# Web UI Code
This is demo version\
[buffetProject_240516](./anylabeling.md)

This is final version (it delete redundant code from buffetProject240516)\
[buffetProject_241201](https://drive.google.com/drive/folders/1F4wTsTuuHcQjv1ANcS9yVGLJcu8D9VdE?usp=drive_link)

# Anylabeling
[anylabeling.md](./anylabeling.md)

