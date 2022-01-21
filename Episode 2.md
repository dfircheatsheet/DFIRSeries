# Intro To Data Acquisition 



## Volatile and non volatile Data:

### Volatile Data :	

 ​	it's the type of data that requires power to maintain the stored information and once the power source is disconnected all the data gets wiped with no way to recover it 

#### Example :

- Ram 
- Registers

### Non Volatile data  :	

​		 it's the type of data that doesn't require power to maintain the stored information 

#### Example:

- Hard Disk
- USB Sticks

## Imaging methods

### Live :

​	Capturing the data while the operating system is running using tools like " FTK imager "

### Static AKA (Dead box acquisition):

​	Capturing the data without running the OS by connecting the Hard disk to other devices or using tools like "Write blocker"

### Local:   

​	means you have physical access to the device and you can install the tools you need directly to the device 

### Remotely:

​	using another device on the network to get the data from the infected device 

## Image file formats

### Images:

- E01: Stores the metadata of the files, also does a compression to make the size smaller and easy to move 
- Raw: just a copy of the data, and you will need to save the metadata into a text file beside the data that will help you understand when the file was created or accessed and create a timeline for the attack 

### Containers:

​	type of acquisition that takes only parts of the hard disk and that will be faster if you have a specific part that you need to investigate also it stores the metadata like:
- AD1
- VHD

## Data verification 

​	Hashing is the best way to verify the acquired image any change in the data will give a different hash
some of the acquisition tools save the hashes in the image after completing the acquisition so it makes it easy for you to verify the data and make sure nothing got changed or missed while the acquisition
