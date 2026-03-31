REFLECTION.md                                                                          
                                                                                           
This commit introduces an implementation for the "Hunter's Mark" effect. It is important to
note that the original maintainer was aware of this feature but deemed it impractical to   
implement directly for all spells.                                                         
                                                                                           
Adding all spells to the `Character` class would create a significant dependency on the D&D
Beyond website's ever-changing DOM structure. This approach would require constantly       
updating the extension to adapt to site changes, making it difficult to maintain stability.
                                                                                           
Instead, a more flexible workaround for handling spells exists by utilizing custom rolls   
and custom hotkeys, allowing users to define specific spell effects without hardcoding     
every spell into the extension's logic.     