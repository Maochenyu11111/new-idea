list = [5,7,11,22,27,33,39,52,58]
erfen = 0
def binary_search(number,left,right):
  if left<=right:
    middle =(left+right)//2
    #中间或靠左
    if number < list[middle]:
      right = middle-1
    elif number >list[middle]:
      left = middle+1
    else:
      return middle
    return binary_search(number,left,right)    
