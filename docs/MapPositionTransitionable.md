<a name="module_MapPositionTransitionable"></a>
##MapPositionTransitionable([position])

The MapPositionTransitionable makes it possible to transition between two geographical
positions. Currently, only standard transition definitions are supported (see `Transitionable`), but in the future more interesting
transitions may be added.

*This class is used internally by `MapView` and `MapStateModifier`.*

**Params**
- [position] `LatLng` - Default geopgraphical position

  
**Contents**  
* [setDefaultTransition(transition)](#module_MapPositionTransitionable#setDefaultTransition)
* [reset(position)](#module_MapPositionTransitionable#reset)
* [set(position, [transition], [callback])](#module_MapPositionTransitionable#set)
* [get()](#module_MapPositionTransitionable#get)
* [getFinal()](#module_MapPositionTransitionable#getFinal)
* [isActive()](#module_MapPositionTransitionable#isActive)
* [halt()](#module_MapPositionTransitionable#halt)

<a name="module_MapPositionTransitionable#setDefaultTransition"></a>
###mapPositionTransitionable.setDefaultTransition(transition)
Sets the default transition to use for transitioning between position states.

**Params**
- transition `Object` - Transition definition

<a name="module_MapPositionTransitionable#reset"></a>
###mapPositionTransitionable.reset(position)
Cancel all transitions and reset to a geographical position.

**Params**
- position `LatLng`

<a name="module_MapPositionTransitionable#set"></a>
###mapPositionTransitionable.set(position, [transition], [callback])
Set the geographical position by adding it to the queue of transition.

**Params**
- position `LatLng`
- [transition] `Object` - Transition definition
- [callback] `function` - Callback

<a name="module_MapPositionTransitionable#get"></a>
###mapPositionTransitionable.get()
Get the current geographical position.

**Returns**: `LatLng`  
<a name="module_MapPositionTransitionable#getFinal"></a>
###mapPositionTransitionable.getFinal()
Get the destination geographical position.

**Returns**: `LatLng`  
<a name="module_MapPositionTransitionable#isActive"></a>
###mapPositionTransitionable.isActive()
Determine if the transitionable is currently transitioning

**Returns**: `Boolean`  
<a name="module_MapPositionTransitionable#halt"></a>
###mapPositionTransitionable.halt()
Halts the transition

