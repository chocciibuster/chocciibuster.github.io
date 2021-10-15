
# States

The `State` class defines the states the state machine can be in.

```gdscript
"""
Base interface for all states: it doesn't do anything in itself
but forces us to pass the right arguments to the methods below
and makes sure every State object had all of these methods.
"""
extends Node

signal finished(next_state_name)

func enter():
	"""
	What happens when you enter the state
	"""
	return

func exit():
	"""
	What happens when you exit the state
	"""
	return

func handle_input(event):
	"""
	What happens when you receive input while in this state
	"""
	return

func update(delta):
	"""
	What happens every frame that you are in this state
	"""
	return

func _on_animation_finished(anim_name):
	return
```
