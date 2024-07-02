### Naming Conventions in C#

Naming conventions in C# help ensure code consistency and readability. Here are the commonly accepted conventions for various elements in C#:

#### 1. Pascal Case (PascalCasing)
Used for:
- Class names
- Struct names
- Enum names
- Public methods
- Properties
- Events

**Examples:**
```csharp
public class CustomerOrder { }
public struct OrderDetail { }
public enum OrderStatus { Pending, Shipped, Delivered }
public void ProcessOrder() { }
public string CustomerName { get; set; }
public event EventHandler OrderProcessed;
```

#### 2. Camel Case (camelCasing)
Used for:
- Private or internal fields
- Parameters
- Local variables
- Method arguments

**Examples:**
```csharp
private int orderId;
private string customerName;
public void ProcessOrder(int orderId, string customerName) { }
```

#### 3. Uppercase (ALL_CAPS)
Used for:
- Constants

**Examples:**
```csharp
public const int MAX_ORDERS = 100;
public static readonly string DEFAULT_CATEGORY = "General";
```

#### 4. Underscore Prefix (_camelCase)
Used for:
- Private fields (optional, but common to avoid conflicts with method parameters or properties)

**Examples:**
```csharp
private int _orderId;
private string _customerName;
```

#### 5. Interface Names (PascalCasing with "I" Prefix)
Used for:
- Interface names

**Examples:**
```csharp
public interface IOrderProcessor { }
public interface IRepository<T> { }
```

#### 6. Namespace Names (PascalCasing)
Used for:
- Namespaces

**Examples:**
```csharp
namespace MyCompany.Project.Module
{
    public class MyClass { }
}
```

#### 7. File Names (PascalCasing)
Used for:
- File names should match the class name

**Examples:**
- `CustomerOrder.cs` for the `CustomerOrder` class.
- `OrderProcessor.cs` for the `OrderProcessor` class.

#### 8. Attribute Names (PascalCasing with "Attribute" Suffix)
Used for:
- Attributes

**Examples:**
```csharp
public class SerializableAttribute : Attribute { }
public class RequiredAttribute : Attribute { }
```

#### 9. Method Parameter Names (camelCase)
Used for:
- Method parameters

**Examples:**
```csharp
public void ProcessOrder(int orderId, string customerName) { }
```

#### 10. XML Documentation Tags (CamelCase)
Used for:
- XML documentation comments

**Examples:**
```csharp
/// <summary>
/// Processes the order.
/// </summary>
/// <param name="orderId">The order identifier.</param>
/// <param name="customerName">Name of the customer.</param>
public void ProcessOrder(int orderId, string customerName) { }
```

### Summary of Conventions
| Element               | Convention     | Example                      |
|-----------------------|----------------|------------------------------|
| Class/Struct/Enum     | PascalCase     | `CustomerOrder`              |
| Interface             | PascalCase + I | `IOrderProcessor`            |
| Method                | PascalCase     | `ProcessOrder`               |
| Property              | PascalCase     | `CustomerName`               |
| Event                 | PascalCase     | `OrderProcessed`             |
| Constant              | ALL_CAPS       | `MAX_ORDERS`                 |
| Private Field         | _camelCase     | `_orderId`                   |
| Local Variable        | camelCase      | `orderCount`                 |
| Parameter             | camelCase      | `orderId`                    |
| Namespace             | PascalCase     | `MyCompany.Project.Module`   |
| File Name             | PascalCase     | `CustomerOrder.cs`           |
| Attribute             | PascalCase     | `SerializableAttribute`      |
| XML Doc Tags          | PascalCase     | `<summary> ... </summary>`   |

