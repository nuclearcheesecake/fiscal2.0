# FISCAL 2.0 - UX-driven actuarial calculator built using C#

<p align="center">
  <img width="415" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/Screenshot%202022-02-02%20120403.png">
</p>

## Table of Contents

* [Background](#1)
* [FISCAL 1.0 in Excel](#2)
* [Presenting FISCAL 2.0](#3)
  - [Project PowerPoint](#4)
  - [GeeXpo presentation](#5)
* [Explanation of functionality](#6)
  - [Home page](#7)
  - [Converting interest rates](#8)
  - [Single Investments](#9)
  - [Annuities](#10)
  - [Loans](#11)
  - [Amortization Tables](#12)
* [Conclusion](#13)

<a name="1"></a>
# Background

I think that most programmers look back at their first large project with a mix of nostalgia for a simpler time and a healthy amount of gratitude that we have grown past the use of spaghetti code. 

I am no exception to this thought. 

FISCAL was my first real project. At the time, I was just starting my journey down the path made of codeblocks. I had serious doubts as a programmer, since prior to my degree, the world of programming was foreign to me, and suddenly, I had this daunting task of creating a functional application - that can leverage financial mathematics!

I remember the endless nights in my dorm room, stretched over two months, pouring over documentation. And then a quick walk to my friend's room to vent my frustration, and then back at the computer, reading and coding. And then...suddenly, success. 

This application formed a part of my financial mathematics modules, and we were required to build a system that can perform actuarial calculations. Most people completed this task in Excel, but at the same time, I was busy with another module in Graphical User Interfaces, where we created small apps in Visual Studio 2017 using C#. Quickly the idea formed to streamline the user experience using this technology, instead of Excel which, albeit powerful, did not have the interface functionality I desired.

Thus the **Financial Solidarity Calculator**, or FISCAL, was born. 

User Experience (UX) was a big focus for me, and the design was always kept in mind when coding. The decision to move to C# is justified then, looking at the...interesting design capabilities I had in Excel at the time. My design in C# is also not very sleek or modern, but I still get the warm fuzzies, knowing a lot of thought went into every button on every page. 

This project was a milestone in my early development, and I'm happy to share it with you today.  

<a name="2"></a>
# FISCAL 1.0 in Excel

I, like my peers, started this project in Excel. Albeit horrendously ugly, as seen below, this simple layout inspired my further designs for FISCAL's homepage. Each button takes you to the specific actuarial function that needed to be performed:

<p align="center">
  <img width="850" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/1.png">
</p>

Here, for example, is a simple flow, where the user would decide the specific parameters, which eventually redirected them to a screen where they could input data:

<p align="center">
  <img width="600" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/2.png">
</p>

<p align="center">
  <img width="600" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/3.png">
</p>

<p align="center">
  <img width="850" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/4.png">
</p>


<a name="3"></a>
# Presenting FISCAL 2.0

<p align="center">
  <img width="415" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/6.jpg">
</p>

Improving, in my sensibilities at least, on 1.0, FISCAL 2.0 created a more streamlined UX with stronger programming power. Below are the pitches for the product, which I had to give in two different contexts. Let's look at that before we explore FISCAL 2.0, just to see if my presentations would have sold the idea to you at the time. 

<a name="4"></a>
## Project PowerPoint

Firstly, I had to present the project to my lecturers. Here are the most important slides in this presentation;

<p align="center">
  <img width="700" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/5.png">
</p>

<p align="center">
  <img width="700" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/present1.png">
</p>

<p align="center">
  <img width="700" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/present2.png">
</p>

<p align="center">
  <img width="700" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/present3.png">
</p>

<a name="5"></a>
## GeeXpo presentation

Each year, our campus held GeeXpo, an exhibition of IT talent and possibilities. Students from various surrounding high schools are invited to come take part in competitions, attend seminars and see what the world of studying tech holds for them. I was asked to present FISCAL 2.0 to a group of students. Little did I know I'd be the last to make such a presentation, due to the pandemic hitting the next year, but that is unimportant for this story. 

Here is a poster for the 2019 event:

<p align="center">
  <img width="415" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/7.png">
</p>

And here are my most important slides. I ended up pitching the importance of data science in our society way more than showcasing my project, but hey, trying to stop a data science student when he is passionate about his work is a cardinal sin. 

<p align="center">
  <img width="700" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/present4.png">
</p>

<p align="center">
  <img width="700" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/present5.png">
</p>

<p align="center">
  <img width="700" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/present6.png">
</p>

<a name="6"></a>
# Explanation of functionality

Early days, spagetti code eg.

```C#
else
{
  if (Global.LANG_GERMAN == false && Global.LANG_AFR == false)
  {
    if (MessageBox.Show("Continue without entering your username?", "Continue?", MessageBoxButtons.YesNo) == DialogResult.Yes)
    {
      if (tutorial == false)
      {
        this.Hide();
        Form1 f1 = new Form1();
        f1.Show();
      }
      else if (tutorial == true)
      {
        Form15 f15 = new Form15();
        f15.Show();
        this.Hide();
       }
     }
  }
    else if (Global.LANG_AFR)
    {
       if (MessageBox.Show("Gaan voort sonder om gebruikersnaam in te sleutel?", "Gaan voort?", MessageBoxButtons.YesNo) == DialogResult.Yes)
       {
          if (tutorial == false)
           {

              this.Hide();
              Form1 f1 = new Form1();
              f1.Show();
           }
           else
           {
              Form15 f15 = new Form15();
              f15.Show();
              this.Hide();
           }
         }
       }
       else
       {
           if (MessageBox.Show("Fahren Sie fort, ohne einen Benutzernamen einzugeben?", "Fortsetzen?", MessageBoxButtons.YesNo) == DialogResult.Yes)
           {
              if (tutorial == false)
              {
                   this.Hide();
                   Form1 f1 = new Form1();
                   f1.Show();
               }
               else
               {
                   Form15 f15 = new Form15();
                   f15.Show();
                   this.Hide();
                }
          }
    }
                    
  }
}
```

<a name="7"></a>
## Home page

<p align="center">
  <img width="500" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/8.png">
</p>

<p align="center">
  <img width="500" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/9.png">
</p>

<p align="center">
  <img width="500" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/10.png">
</p>

- Languages
- User with password, but can continue without
- Save information 
- Tutorial option
- Printing session

<p align="center">
  <img width="415" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/11.png">
</p>

<p align="center">
  <img width="500" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/12.png">
</p>

<p align="center">
  <img width="500" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/13.png">
</p>

<p align="center">
  <img width="500" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/31.png">
</p>

<p align="center">
  <img width="300" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/14.png">
</p>

<p align="center">
  <img width="500" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/15.png">
</p>

<p align="center">
  <img width="500" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/16.png">
</p>

<a name="8"></a>
## Converting interest rates

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/17.png">
</p>

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/18.png">
</p>

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/32.png">
</p>

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/19.png">
</p>

<a name="9"></a>
## Single Investments

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/22.png">
</p>

<p align="center">
  <img width="400" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/20.png">
</p>

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/21.png">
</p>

<a name="10"></a>
## Annuities

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/23.png">
</p>

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/24.png">
</p>

<a name="11"></a>
## Loans

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/25.png">
</p>

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/26.png">
</p>

<a name="12"></a>
## Amortization Tables

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/30.png">
</p>

<p align="center">
  <img width="350" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/27.png">
</p>

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/28.png">
</p>

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/29.png">
</p>

<a name="13"></a>
# Conclusion

In the end, I scored 95% for this assignment, and was pleased that my first rabbit hole into application programming was recognised.

<p align="center">
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/Screenshot%202022-02-02%20130324.png">
</p>

At the inter-campus competition, FISCAL 2.0 obtained a second place. I am proud of my silver medal - it proved to me that coding only needs guts and an internet connection to master.
