# Arrays

> Time complexity - we look at worst case for **Big O notation**
---

## Operations
Few operations and time complexity in Big O notation

#### Indexing 
* O(1) / constant time

#### Seach/ lookup by value 
* O(n) element at end of list
* Works as : initial_memory_loc + fetch_idx * size of data type 
* E.g `0x00500 + 2 * 4` gives 2nd element mememory loc and int is of 4 bytes.

#### Print a value / Traversal
* O(n) - Element at end of list

#### Insert / Delete a element
* After insertion/ deletion of element in given index position , the remaining value will shift
* Use `l.insert(idx, value)` to insert an element.
* use `l.pop(), l.remove(value), l.delete(idx, value)` to delete an element
* O(n) - where n is no of swaps

---

## Dynamic vs Static Array
Difference and working of Dynamic vs Static array

### Static Array
* Length of array is not changed thus inserting new element after assinged len can give errors
* Only allocates memory of fixed size.
* Commonly found in java , c , c++.
* One need to define the length of array previously.
* Example:

```
int[] arr_name = new dtype[arr_len]

arr_name[idx1]= value
.
.
arr_name[idxN]= value
```


### Dynamic Array
* Length can decrease with removal or addition of element
* First allocate a default memory area / size, once that size / len is reached , uses algorithm `current_cap + current_cap*2 / GP` to allocate new space(memeory location) and copy the previous array element to new memeory location.






