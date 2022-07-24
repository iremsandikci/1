# 1 i = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]

temp = []
def flatten(input):
  
  if(type(input)==list):
      for i in input:
        flatten(i)
        
  else:
    temp.append(input)
  return temp
print(flatten(i))


input = [[1, 2], [3, 4], [5, 6, 7],[9,10,11]]

temp = []
def reverse(arr):
  for item in arr[::-1]:
    if item==list:
      reverse(item)
    else:
      temp.append(item[::-1])
  return temp

print(reverse(input))
