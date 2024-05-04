# Tutorial 10 ༘⋆🌷🫧💭₊˚ෆ
## Nabiilah Putri Safa
----------------------

## 1.2 Understanding how it works

![Screenshot 2024-05-04 120754](https://github.com/nabiilahputri13/my-first-repob/assets/124870275/78eab566-d1ed-4644-b583-0086dea95914)

From the observed output, it can be understood that the async function will run outside of the main function that invokes it. Therefore, "hey hey" might be outputted before "howdy!" and "done!" because "hey hey" is outside the async function, which allows the function to continue executing and print "hey hey" while the async function is still waiting for the result from the future.

## 1.3: Multiple Spawn and removing drop

![Screenshot 2024-05-04 121534](https://github.com/nabiilahputri13/my-first-repob/assets/124870275/1dc249ce-da5d-4f38-a96a-9c57e607ce75)

From the generated output, it can be observed that having multiple spawners results in more tasks being executed because more tasks are enqueued into the task sender, which acts like a message queue. The non-dropping of spawners causes the program to never terminate because the program assumes that there will still be data sent by the spawner. Dropping the spawner indicates that the interaction is finished and the spawner will be closed. When a spawner calls the spawn function, a new task is created and pushed into the task sender. The executor retrieves one task from the task sender, executes it, and then retrieves more tasks until there are no tasks left, and finally, the spawner is dropped, signifying the end of the interaction.