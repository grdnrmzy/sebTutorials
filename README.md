# Sebastian's tutorials

[kmfmd](#E7)

**E1.**


Variable - name to which data can be assigned.


| var    | example                  |
| -------- | -------------------------- |
| int    | playerHealth = 15;       |
| float  | playerHealth = 15f;      |
| bool   | playerHealth = true;     |
| string | playerHealth = 'health'; |

Functions means a specific task, so that it can be called from multiple places.

---

**E2.**

Classes  = var + functions.

Inheritance

![20210823_111826_20210823_111813_Untitled.png](assets/20210823_111826_20210823_111813_Untitled.png)

Composition

![20210823_112522_20210823_112510_0_J_Dm57bKTppN51oZ.png](assets/20210823_112522_20210823_112510_0_J_Dm57bKTppN51oZ.png)

**Formally, “instance” is synonymous with “object” as they are each a particular value (realization), and these may be called an instance object; “instance” emphasizes the distinct identity of the object. The creation of an instance is called instantiation.**

---

**E3.**

Overview of Unity interface.

![20210823_115804_image.png](assets/20210823_115804_image.png)

---

**E4.**
Writting code for getting distance between 2 points.

---

**E5.**

operators and if statements.

**% - The remainder operator % computes the remainder after dividing its left-hand operand by its right-hand operand.**

``` csharp
Console.WriteLine(**5** % **4**);   **// output: 1**
Console.WriteLine(**5** % **-4**);  **// output: 1**
Console.WriteLine(**-5** % **4**);  **// output: -1**
Console.WriteLine(**-5** % **-4**); **// output: -1**
```

---

**E6.**
simple game with `public class TimeGame;`

---

## E7

vectors:

vector2 - for 2d;

vector3 - for 3d;

---
## E8
![e8.png](assets/e8.png)

adding movement intro game.

---
## E9

writting roration script.

```csharp
public class CubeScript : MonoBehaviour {
    public Transform sphereTransform;

    void Start(){
        sphereTransform.parent = transform;
    }

    void Update(){
        transform.eulerAngles += new Vector3 (0, 180 * Time.deltaTime, 0);
    }
}
```
Use Transform.Rotate to rotate GameObjects in a variety of ways.

---

## E10

collision (столкновение).
Collisions in Unity are separated from the actual Sprite itself, attached as separate components and are calculated on their own.

**Everything** in game is GameObject.
