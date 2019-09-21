# **Enscapsulation- _Problem4:First and Reserve Team_**
## **Problem 04**
### _**First and Reserve Team**_
> _**NOTE:**_ Creating a public _**Startup**_ class with the namescape _**PersonInfo**_.  
Create s _**Team**_ class. Add to this team all of the people you have received. Those who are younger than 40 go to the first team, others fo to the reserve team. At the end print the sizes of the first and the reserved team.  
The class should have _**private fiels**_ for:
* name : string  
* firstTeam : List`<Person>`
* reserveTeam: List`<Person>`  

The class should have _**constructors**_:
* Team(string name)  

The class should also have _**public properties**_ for:
* FirstTeam : List`<Person>` (read only!)
* ReserveTeam : List `<Person>` (read only!)

And a method for adding players:
* AddPalyer(Person person): void  

## **Input and Output**
**Input** | **Output**
----------|-----------
5 | First team has 4 players.
Asen Ivanov 20 2200 | Reserve team has 1 players.
Boiko Borisov 57 3333 |
Ventsislav Ivanov 27 600 |
Grigor Dimitrov 25 666066 |
Boiko Angleov 35 555 |

## **Solution**
1. Using the _**Person**_ class that created in the previous tasks.
2. Adding a new class _**Team**_. Its fields and constructor shown as the following figure.
   ![Imgur](https://i.imgur.com/rZzqIWZ.png)  

3. Properties for FirstTeam and ReserveTeam have only getters. In this section, we using _**IReadOnlyCollection**_ to protect the data and this collection should be treated as immutable, and the client code shoukd onky read it, and not update it.
   ![Imgur](https://i.imgur.com/P5n0hQI.png)   
   
4. There will have method, which adds players to teams.
   ![Imgur](https://i.imgur.com/bofGeoE.png)  

5. Adding ToString() methods into _**Team**_ class.  
   ![Imgur](https://i.imgur.com/vh2uqyU.png)  
6. In the _**Program.cs**_, we create a new team with name _**GCD0819**_
   ![Imgur](https://i.imgur.com/VfSdRTU.png)  

7. Using _**for**_ loops to input the objects to the team and calling _**AddPlayers**_ method to classify. Besides that, within the loops we using the _**try..catch**_ statement to find the exceptions and handle this by show the messages.  
   [Imgur](https://i.imgur.com/Prkg0H2.png)  

8. To display the sizes of both of team, we calling _**ToString()**_ method.
   ![Imgur](https://i.imgur.com/0yQYQK8.png)  

## **The result**
![Imgur](https://i.imgur.com/kEmIhBX.png)
