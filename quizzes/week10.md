# C# Fundamentals


**1.** What is the purpose of a `namespace`?
<!-- enter you answer in the space below -->
```
namespace allows access to files without needing to import it
```
**2.** What is the difference between a `class` and a `struct`?
<!-- enter you answer in the space below -->
```
class: reference type; struct: value type
```
**3.** What is the method that returns an instance of a class, yet it has no return type?
<!-- enter you answer in the space below -->
```
void
```
## Example 1
```c#
abstract class Car
{
  ...
  public virtual string Start()
  {
    return "Vroooom";
  }
}
```
**5.** In the example what is the access modifier of the `Start()` method?
<!-- enter you answer in the space below -->
```
public
```
**6.** In the example what is `string` an indication of?
<!-- enter you answer in the space below -->
```
type that will be returned
```
**7.** In the example what is `abstract` preventing?
<!-- enter you answer in the space below -->
```
indicates a modifier that is incomplete or missing implementation
```
**8.** In the example what is the purpose of `virtual`?
<!-- enter you answer in the space below -->
```
implement the base class of the method
```
**9.** Name four access modifiers:
<!-- enter you answer in the space below -->
```
private, public, protected, internal,
```
**10.** If you set a class or method to private, what can access it?
<!-- enter you answer in the space below -->
```
items within the class
```