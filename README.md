# Tutorial 10
# Nabiilah Putri Safa
----------------------

## 1.2 Understanding how it works

![Screenshot 2024-05-04 120754](https://github.com/nabiilahputri13/my-first-repob/assets/124870275/78eab566-d1ed-4644-b583-0086dea95914)

From the observed output, it can be understood that the async function will run outside of the main function that invokes it. Therefore, "hey hey" might be outputted before "howdy!" and "done!" because "hey hey" is outside the async function, which allows the function to continue executing and print "hey hey" while the async function is still waiting for the result from the future.