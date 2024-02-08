#       Collections in Apex 
                             
  1. List 

- Example:

         List<Integer> numbers = new List<Integer>();                                       // any data type can be used here as per the requirement
         numbers.add(1);                                                                    // add is used to add any value to List
         numbers.add(1);
         numbers.add(2);
         numbers.add(3);
         System.debug('List of numbers: ' + numbers);
         output => 1 1 2 3                                                                 // duplicate values are allowed in List
            
          
 2. Set
          
-  Example:
  
          Set<Integer> numbers = new Set<Integer>();                                       // any data type can be used here as per the requirement
          numbers.add(1);                                                                  // add is used to add any value to Set
          numbers.add(1);                    
          numbers.add(2);
          numbers.add(3);
          System.debug('Set of numbers: ' + numbers);
          output => 1 2 3                                                                 // duplicate values are not allowed in Set
          
          
3. Map
          
- Example:
  
          Map<Integer, String> mapOfIntegerAndString = new Map<Integer, Stirng>();       // any data type can be used here as per the requirement
          mapOfIntegerAndString.put(1, 'One');                                           // put is used to add any value to Map
          mapOfIntegerAndString.put(2, 'Two');
          mapOfIntegerAndString.put(3, 'Three');
          mapOfIntegerAndString.put(3, 'Four');
          System.debug('Map Of Integer And String: ' + mapOfIntegerAndString);
          output => 1=One, 2=Two, 3=Four                                                // duplicate values are not allowed in Map so it will overwrite the last value in this case => 3, Three
          






