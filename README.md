# Circular Buffer

Data structure that holds a fixed amount of items of a specific data type. It's designed more for managing history, such as undo-redo functionality, therefore it allows you to overwrite the items after moving backward in order to discard the "redo" history.

- Supports committing new items, and moving backward and forward through them.

- When the buffer is full the wrapping occurs and the oldest items are overwritten.

- After moving backward, new commits will overwrite the items ahead of the current pointer.

- Suitable for undo-redo implementations like history management.
