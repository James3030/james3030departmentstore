# james3030departmentstore
Location finder for items within a department store

floors = {
 "lower": ["clothes", "food"], 
 "upper": ["sports", "shoes"],
 "basement": ["gardening", "furniture"]
 }

found = False
requested = "food"
current = "upper"

if requested in floors[current]:
 print("Yes, on this floor.")
 found = True

else:

 for floor in ["lower", "upper", "basement"]:
   if requested in floors[floor]:
    print("On " + floor + " floor.")
    found = True
    
if found == False:
 print("Sorry, not sold in this store.")
