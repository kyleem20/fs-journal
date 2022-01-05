# CSHARP
On Final: create profile model of 3 items

async Task<>
 



instantiate variables in c#: string str = Start()
public ... int, double, float, decimal, string
Lists - used in place of an array
System.Collections.Generic : List<string>

dotnet new webapi -n PROJECTNAME

? = can accept a null input

prop tab = public builder
constainskey is important!
: - inheritance: extends
static: class is always available, cannot be instantiated (no new ...)
<> : of type

users: create new user
host:= connection endpoints
username: user you created
connect

KyleeDB: >
Table: Create Table, (table : collection);
[name] => collection name



launch.json: "ASPNETCORE_URLS": "https://localhost:5001"
change .env baseURL

IEnumerable: and type of collection

204: succeeded but got nothing back, no context

___ViewModel: created for the many to many relationships
----
Warm Up:
Console.Clear();
Dictionary<string, User> users = new Dictionary<string, User>(){
  {"mark", new User("mark", "IHeartCod3")}
};

users.Add("Mick", new User("Mick", "ISecretlyHateCss"));
users.Add("Jake", new User("jake", "CodingIsRFun"));





Console.WriteLine("Welcome, please enter your username: ");
string? username = Console.ReadLine();
Console.WriteLine("Please enter your password: ");
string? pass = Console.ReadLine();

if(users.ContainsKey(username) && users[username].isValidPassword(pass)){
  System.Console.WriteLine("It WORKS!!!");
}else {
  System.Console.WriteLine("fail!");
}


-------
Build a console app where you roll dice. Roll two dice, three times. If any of the sets are equal (6 and 6 or 1 and 1, etc) your score is 0. Otherwise print the dice rolls and the sum of the dice.

Dice:

Program:



