<div align="center">

## Bubble sort


</div>

### Description

An implementation of bubble sort alghoritem.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[cime2007](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/cime2007.md)
**Level**          |Beginner
**User Rating**    |3.0 (9 globes from 3 users)
**Compatibility**  |C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Algorithms](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/algorithms__3-29.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/cime2007-bubble-sort__3-11122/archive/master.zip)





### Source Code

```
<pre>#include <iostream>
using namespace std;
void PrintArray(int[], int);
void BubbleSort(int[], int);
void Swap(int&, int&);
int main(int argc, char** argv){
  int const arraySize = 8;
  int ourArray[arraySize] = {657,56,4,93,5646,767,5,96};
  //array before sorting
  PrintArray(ourArray, arraySize);
  //sort array
  BubbleSort(ourArray, arraySize);
  //array before after
  PrintArray(ourArray, arraySize);
	return 0;
}
void PrintArray(int array[], int arraySize){
  for (int i=0; i < arraySize; i++){
    cout << array[i] << " ";
  }
  cout << endl;
}
void BubbleSort(int array[], int arraySize){
  bool swaped=true;
  do{
    swaped = false;
    for (int i=0; i < (int)sizeof(array); i++){
      if(array[i] > array[i+1]){
        Swap(array[i], array[i+1]);
        swaped = true;
      }
    }
  }while(swaped);
}
void Swap(int& first, int& second){
  int tmp = first;
  first = second;
  second = tmp;
}
</pre>
```

