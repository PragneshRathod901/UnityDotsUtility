# Different Forces Comparison of UnityEngine and Dots Physics

Index | UnityEngine Physics | Dots Physics | Description
--|:---| :--- | :---
1|`rb.AddForce(ForceMode.Impulse)` | `PhysicsWorld.ApplylinearImpulse()` |Apply impulse to rigidBody using its mass
2|`rb.AddForce(ForceMode.Force)` | **`PhysicsWorld.ApplyLinearForce()`** |Apply continuous force  to rigidBody using its mass
3|`rb.AddForce(ForceMode.acceleration)` | **`PhysicsWorld.ApplyLinearAcceleration()`** |Apply continuous acceleration  to rigidBody ignoring its mass
4|`rb.AddForceAtPosition(ForceMode.Impulse)` | `PhysicsWorld.ApplyImpluse()` |Applies force at position using its mass. As a result this will apply a torque and force on the object 
5|`rb.AddForceAtPosition(ForceMode.acceleration)` | **`PhysicsWorld.ApplyAccelerationImpulse()`** |Applies force at position ignoring its mass. As a result this will apply a torque and force on the object
6|`rb.AddTorque(ForceMode.Impulse)` | `PhysicsWorld.ApplyAngularImpulse()` |Apply torque  to rigidBody using its mass
7|`rb.AddTorque(ForceMode.Force)` | **`PhysicsWorld.ApplyAngularForce()`** |Apply continuous torque   to rigidBody using its mass
8|`rb.AddTorque(ForceMode.acceleration)` | **`PhysicsWorld.ApplyAngularAcceleration()`** |Apply continuous torque   to rigidBody ignoring its mass



### Note:- Bold marked Function Uses [PhysicsorldExteded](https://github.com/PragneshRathod901/UnityDotsUtility/blob/master/DotsPhysics/PhysicsWorldExtended.cs) Script From this Repository