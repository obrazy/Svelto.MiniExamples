# Svelto.ECS.MiniExamples

New Mini Examples for Svelto.ECS.

* Svelto.ECS: https://github.com/sebas77/Svelto.ECS

These examples use the last beta version of unity available at the moment of the update.

Warning: these examples may use using unofficial versions of Svelto that you won't find on the main repository until officially released.

## 🔴Example 1: Doofuses Must Eat (Unity Version)🔴

![Image](https://github.com/sebas77/Svelto.MiniExamples/blob/master/2020-12-22%2016-05-22.gif)

Object-less pure ECS example that shows the basics of Svelto.ECS. 

Attention this demo is presented in multiple versions thanks to its flexibility. **this demo is for advanced users, other demo are less overwhelming**

Article:

http://www.sebaslab.com/svelto-mini-examples-doofuses-must-eat/ (obsolete now, new article incoming)

### Goals of the **SveltoOnDOTS** example are to: 
* intoduce to the concept of entity descriptors, entity structs and groups. 
* Show the integration with DOTS ECS, shows the use of Svelto.Tasks 2.0 (alpha state) 
* show the integration with DOTS Jobs and Burst (using Svelto.ECS 3.0)
* test Full jobified/burstified code with Svelto ECS 3.0
* test integration with IL2CPP

### Goals of the **GameObjects** example are to: 
* show how the OOP abtraction layer works (https://www.sebaslab.com/oop-abstraction-layer-in-a-ecs-centric-application/)
* show how the resource managers work to interface objects and entities 
* show that even with OOP interfacing, ECS helps to achieve high performance

## 🔴Example 1: Doofuses Must Eat (Stride Version)🔴

### Goals of the **Stride example** are to: 
* show a complex integration with an engine different than Unity (Stride Engine)

### Goals of the **Stride Compute Sharp example** are to
* Goal: show how to extend internal Svelto datastructure to customise data storage
* Goal: show how to run c# svelto engines on the GPU (automatically converted to compute shader by ComputeSharp)
* article https://www.sebaslab.com/svelto-ecs-3-4-internals-how-to-integrate-computesharp/
  
## 🔴Example 2: The classic Survival demo (Hybrid ECS)🔴

![Image](https://github.com/sebas77/GithubWikiImages/blob/master/gif_animation_002.gif)

Basic integration with Unity GameObjects and Monobehaviours.

main article: https://www.sebaslab.com/the-new-svelto-ecs-survival-mini-example/

Goal of this example: 

* show the integration with OOP platforms (Unity in this case) throught the use of OOP abstraction layers.
* *Test WebGL support*

I used the Survival Shooter Unity Demo to show how an ECS framework could work inside Unity. I am not sure about the license of this demo, so use it only for learning purposes.
Most of the source code has been rewritten to work with Svelto.ECS framework. The Survival Demo is tested with the latest version of Unity, so I cannot guarantee that it always works.

* Note: The purposes of this demo is NOT to show how to write fast code. In fact most of the solutions you will find in this demo may not be optimal. Svelto ECS is used only to wrap high level code as all the low level functionalities are executed through standard gameobjects.

## ~~Example 3: GUI and Service Layer (Hybrid ECS for GUI)~~

~~Integration with Unity UI and Svelto entities 3.0~~

~~Goal of this example~~

* ~~Show how EntityStreams work to publish data changes.~~ 
* ~~Show how to enable databinding with ExclusiveGroups.~~ 
* ~~Show how to setup a data oriented GUI with nested prefabs.~~ 
* ~~Show a basic usage of the Svelto.Services (https://github.com/sebas77/Svelto.Services)~~

~~Main article: http://www.sebaslab.com/svelto-miniexamples-gui-and-services-layer/~~

UI and ECS is an on going problem to solve. I have some better solutions than what proposed in this example now.

## 🔴Example 4: Pure .net + SDL example🔴

Goal of this example

* Show how to use Svelto outside unity in an advanced scenario
* Show how to use efficently group compounds

  Note: the pattern used here are quite unconvinentional. This demo was made by a Svelto user, but I still mantain it. Not easy to follow.

![Image](https://github.com/sebas77/Svelto.MiniExamples/blob/master/Example4-NET-SDL/2020-12-23%2011-54-54.gif)

## Example 5: Hello World (previously called Vanilla)

Basic Platform Agnostic Svelto.ECS 3.0 example

* Goal: Shows the very foundation of a simple entity and engine logic, without any Unity or other platform dependency (pure .net). This example won't cover all the aspects of SECS, but only the basics.

## 🔴Example 6: Abstract Object Oriented Code🔴

* Goal: this example shows the two main strategies to abstract OOP code. Mixing the two strategies will result in the least boiler plate and fastest code.
* Fist integration wraps gameobjects through the use of EntityViewComponents like seen in MiniExamples 2 Survival. **Attention** EntityViewComponents and Implementors are NOT reccomended to use over the second approach.
* Second integration shows a more efficent approach, where pure ECS is used as much as possible and engines objects are synched only as late as possible.

## 🔴Example 7: Awkward foundation for a possible defense game built with the awesome engine that Stride is🔴

* Goal: showing Svelto working with Stride Engine (svelto can work with any engine that supports c# natively)
* Goal: showing how to use EntityReferences to transform hierarchies
* Foundation of my new article https://www.sebaslab.com/svelto-miniexample-7-stride-engine-demo/

![image](https://user-images.githubusercontent.com/945379/134925979-145e5b0e-fd5d-4562-abc3-07bafca2fbe6.png)

## 🔴Example 8: Run Svelto.Engines on GPU using ComputeSharp🔴

* Goal: show how to extend internal Svelto datastructure to customise data storage
* Goal: show how to run c# svelto engines on the GPU (automatically converted to compute shader by ComputeSharp)
* A better example is found at https://github.com/sebas77/Svelto.MiniExamples/tree/master/Example1-Stride-DoofusesMustEat/DOOFUSES_STRIDE_COMPUTESHARP
* Foundation of my new article https://www.sebaslab.com/svelto-ecs-3-4-internals-how-to-integrate-computesharp/

## 🔴Example 9: Simulation🔴

3 version of this demo are available:

* Unity groups only version
* Unity groups and filters version
* Unity groups and filters version with Burst

* Goal: these demos are interesting because are simple and show properly how to subset entities with filters and groups


