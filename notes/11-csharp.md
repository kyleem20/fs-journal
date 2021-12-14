# CSHARP

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