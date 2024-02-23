# AbstractClass
Implement the following:
1.  ListItem (abstract class)
    -  It has three fields. Two s called and , and an called .protectedListItemrightLinkleftLinkObjectvalue
    -  A constructor that takes an and initialises the field with the parameter that was passed in.Objectvalue
    -  And seven methods:
        -  next(), , , and which are and (see child class for declaration).setNext()previous()setPrevious()compareTo()package-privateabstract
        -  getValue(), takes no parameters and returns its .value
        -  setValue(), takes an and assigns it to .Objectvalue
       
2.  Node (concrete class)
    -  It extends .ListItem
    -  It has a constructor that takes an , then calls its parent constructor with the parameter that was passed in.Object
    -  And five methods which are :package-private
        -  next(), takes no parameters and returns the to its right.ListItem
        -  setNext(), takes a and sets it as its , then it returns .ListItemrightLinkrightLink
        -  previous(), takes no parameters and returns the to its left.ListItem
        -  setPrevious(), takes a and sets it as its , then it returns .ListItemleftLinkleftLink
        -  compareTo(), takes a and compares it to the that called this method. Use from for comparison. If this is greater than the that was passed in, then it should return a number greater than zero. If vice versa, then it should return a number less than zero, and zero if equal.ListItemListItemvalueListItemvaluevalue

3.  MyLinkedList (concrete class)
    -  It implements .NodeList
    -  It has one field of type called .ListItemroot
    -  A constructor that takes a and initialises the field with the newly passed in parameter.ListItemroot
    -  And four methods:
        -  getRoot(), getter for .root
        -  addItem(), takes a and returns if it was added successfully or otherwise. If the item is already present, it doesn't get added. Use to place the item in its proper order.ListItemtruefalsecompareTo()
        -  removeItem(), takes a and returns if it was removed successfully or otherwise. ListItemtruefalse
        -  traverse(), takes the as an argument and does not return anything. If the is it prints out: , otherwise print each value on a separate line.rootrootnullThe list is empty

4.  NodeList (interface)
    -  It has four methods:
        -  getRoot(), , and which are and (see child class for declaration).addItem()removeItem()traverse()package-privateabstract

5.  SearchTree (concrete class)
    -  It implements .NodeList
    -  It has one field of type called .ListItemroot
    -  A constructor that takes a and initialises the field with the newly passed in parameter.ListItemroot
    -  And five methods:
        -  getRoot(), getter for .root
        -  addItem(), similar to . See second TIP below.MyLinkedList
        -  removeItem(), same as .MyLinkedList
        -  performRemoval(), takes two s, the item to be removed and its parent. It doesn't return anything and is declared as . Call this method from when the item is found.ListItemprivateremoveItem()
        -  traverse(), takes the as an argument and does not return anything. It uses recursion to visit all the branches in the tree (Inorder). Print each value on a seperate line.root

