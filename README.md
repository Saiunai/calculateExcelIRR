# Excel IRR Function in Apex
Apex method used to calculate the Internal Rate of Return (IRR) of a given set of double number values.

# History Background
While working on a client project, I was given the task to create an Internal Rate of Return (IRR) apex function in Salesforce. I had no idea as to what IRR was, what it was used for or even how it was calculated. After researching more about it, I found that calculating the IRR of a given set of currency of values was a lot trickier than expected. The reason is it involves constantly guessing the IRR value that would make its equation equal to 0 or as close to 0 as possible. 

Thankfully, great mathematicians like Newphton Raphson and Edmond Halley created root-finding algorithms to make the guessing process faster. Before going through the journey of creating my own IRR method, I researched to see if someone else already created one. Most of the results I found were either overly complicated or difficult to follow. I also noticed that most of them utilized Newphton Raphson's root-finding algorithm which was less efficient than Edmond Halley's iteration.

Thus, this led me to wanting to create my own simpler version of IRR method. I wanted it to be very similar to the IRR function used in Excel. The IRR function in Excel simply takes a set of currency values and calculates the IRR for those values. I also decided to utilize Edmond Halley's root-finding algorithm due to its increased effiency. This method I uploaded here is the end result!

I decided to upload my method to help others who may receive a similar requirement in the future. The code has no outside dependencies besides needing a list of currency values so implementing it in any Salesforce project or org should be very easy.
