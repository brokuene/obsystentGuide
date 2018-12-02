# Guide for Obsystent
This document consists of two main parts:
1. Guide for feature usage - how to use particular feature
2. Configuration of Obsystent - before first use you many need to set up Obsystent.

# Guide for feature usage

To use any of the feature you need to press microphone icon on right bottom and say a *voice command*.
That's it.


For every command there are many synonims supported so you don't have to say exactly the same phrase as described in this guide. To see full example list of possible valid commands visit this [link](https://gist.github.com/brokuene/844a9c34cee97552e2fc5545e30350d0).

## Booking
First you need find free room. Say: *Wyszukaj wolną salkę na 5 minut*. Of coure you can give any duration like *pół godziny*, *godzinę*, *2 godziny*, *3 minuty*.
Then application will show you free rooms.

![Alt text](img/booking1.png?raw=true "Title")

After that you can say *Zarezerwój pokój Hotel* or *Zarezerwój pokój cztery trzydzieści siedem* and Obsystent will create "Ad hoc" meeting in this room as you would manually do it in Outlook. Sit down and feel comfortable, you have reservation now.

## SCC
You just need say: *Zaraportuj 3 piętra*. Of course you can give any number.

## VSTS

1. My tasks

The best is to use Obsystent in front of paper task board but if you don't have any you can see your VSTS tasks by saying *Pokaż moje zadania*

![Alt text](img/vsts1.png?raw=true "Title")

This step is optional.

2. Change status

To change task status say *Zadanie dziewięć jest w trakcie* or *Zadanie dziewięć jest nie zaczęte* or *Zadanie dziewięć jest zrobione*.
If task has a long number you can refer to it by tag by saying *Zadanie B12 jest w trakcie*.
A tag is a standard VSTS tag put on particular task. The only requirement is that tag has to be in format [Big letter][Numbers] like: A1, B22, D33.

3. Revert

To revert / undo last action done in Obsystent on VSTS just say *cofnij ostatnie* and task will be reverted to previous state (status, asigned person), so you don't have to worry about mistakes.

4. Assign task to person

You can assign task to some else by saying *Zadanie dziewięć przypisz do Marka* or "Zadanie B12 przypisz do Piotrka*. Yes, tags are also allowed. For this *MVP* the list of people is predefined to Marek, Piotrek, Arek, Mateusz, Łukasz. Please vote for our project to allow us to add configuration panel.


# Configuration of Obsystent
In settings menu you should fill section related to feature you are interested for.
To use *Booking* you don't need to set anything in configuration.
To use SCC you need only fill in our credentials (the same which are used in website.)
If you want use VSTS please fill VSTS section, but if not needed it is perfectly fine to leave it blank.

**See subsections for more detailed information per feature**

## Configure Room booking
To use *Booking* you don't need to set anything in configuration, on first use a new Browser window will pop-up and ask you for you domain credentials.

## Configure SCC
To use SCC it is esential to fill your nick and credentials used to login into SCC website.

![Alt text](img/ob2.png?raw=true "Title")

## Configure VSTS
Obsystent needs *Access Token* in order to access your VSTS task board. 
To Generate new token please do the following:
![Alt text](img/vstsConfig1.png?raw=true "Title")
![Alt text](img/vstsConfig2.png?raw=true "Title")

![Alt text](img/vstsConfig3.png?raw=true "Title")

A generated token is a long string, best it is to send it via e-mail to mobile phone and paste to Obsystent app.

![Alt text](img/ob1.png?raw=true "Title")

In field *VSTS Project name* put name of project.
In field *VSTS Organization* put organization name.
You can find those values on your VSTS, for me it looks like here:

![Alt text](img/vstsConfig4.png?raw=true "Title")
