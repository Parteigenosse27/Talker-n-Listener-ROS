# Talker-n-Listener-ROS
_In this repository are presented custom ROS packages of message, talker and listener in Python. The main target is to get more practice in working with ROS._

![FirstStep](https://github.com/user-attachments/assets/87444399-e1bf-4af7-932c-049e0f882bd0)

First step is standard creating wokspace and src in the root. After that, `cause of our task to create custom message, we need to create a new package with it. 

_Remark._
_You can name this package as you want._

![SecondStep](https://github.com/user-attachments/assets/0052e54b-7414-4f35-a42c-04d97fcb7891)

To provide a correct work of our package we need to open CMakeLists.txt file in directory workspace/src/my_custom_msg.

![ThirdStep](https://github.com/user-attachments/assets/461042aa-062a-4f8b-9fb9-3a8deb870f1c)

In this file:

1. on 10 line you need to write additional required component message.generation;

![Fourth step](https://github.com/user-attachments/assets/e7245501-13ee-4e8e-aa8e-e625e56311bb)

2. on 49 line uncomment function _add_message_files_;

![StepFive](https://github.com/user-attachments/assets/8fb42c6d-8842-4eda-b3eb-27cec7fed349)

3. on line 70 uncomment function _generate_messages_;

![StepSix](https://github.com/user-attachments/assets/74fbf63d-8faf-49f0-89eb-a87be1329599)

4. also don`t forget to uncomment on 104 line _CATKIN_DEPENDS_;

![StepSeven](https://github.com/user-attachments/assets/b59d4137-86ec-441f-b87d-cdda2497ccef)

Great! Now we save all changes and open _package.xml_ file.

![StepEight](https://github.com/user-attachments/assets/df74b65e-fb0a-4030-a88e-625cf5643109)

![StepEightPointOne](https://github.com/user-attachments/assets/3358f302-aea6-4206-8800-1c7ffcb33864)

In this .xml file you need to add build and runtime dependences by copying commented lines in bulids block.

![StepNine](https://github.com/user-attachments/assets/1753f581-f722-4e7a-b009-44581b30d6e6)

After that we save changes close our kate editor.

So, we ended with configurating with whole package, but we stil don`t have any files about structure of our custom message... 
Let is fix that moment.

In our package directory we need to open Message1.msg. Of course by using kate.

So, we see the white and empty file. And we can write here types of data that we need to send in this message.

From my side of view, the easiest way - write in this file just _string_ with name text.

So, we have ended with package and file in it. Let`s compilate it!

![StepTen](https://github.com/user-attachments/assets/b107c615-c1d1-499c-bb0a-d5c1044ae982)
![StepTenPointOne](https://github.com/user-attachments/assets/8eea5f0a-3f39-4c67-a07c-c7f7c31e8e16)

Great! Everything is working as should.

Now we need to create another package with 2 nodes - talker and listener.

I shall not write here about code in python, you can read more about in .py files.

We do every step that we have been done before to create another package and nodes, so I shall not repeat it here again.

