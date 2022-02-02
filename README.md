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

Looking back at my start as a programmer - this was my first real project. Nostalgia. Doubts as a programmer, daunting task. Endless nights.

Background on module and task

At the same time, I was busy with another module in Graphical User Interfaces, where we created small apps in Visual Studio 2017 using C#. Quickly the idea formed to streamline the user experience using this technology, instead of Excel which, albeit powerful, did not have the interface functionality I desired.

Thus the **Financial Solidarity Calculator**, or FISCAL, was born. 

User Experience (UX) was a big focus for me, and the design was always kept in mind when coding. The decision to move to C# is justified then, looking at the...interesting design capabilities I had in Excel at the time.

<a name="2"></a>
# FISCAL 1.0 in Excel

<p align="center">
  <img width="850" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/1.png">
</p>

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

<a name="4"></a>
## Project PowerPoint

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

<p align="center">
  <img width="415" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/7.png">
</p>

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
  <img width="650" src="https://github.com/nuclearcheesecake/fiscal2.0/blob/main/images/20.png">
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
