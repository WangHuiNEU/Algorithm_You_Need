# Algorithm

> Everyday



# 3/16

## 1.二分查找

```python
class model:
    def search(self,nums:List[int],target:int) ->int：
    	left,right = 0, len(nums)-1
        while(left<=right):
            medium = (right-left)//2 + left
            if nums[medium] == target:
                return medium
            elif nums[medium] > target:
                right = medium - 1
            else:
                left = meidum + 1
        return -1
```

> 二分查找可以记住

## 2.两数之和

> 用字典可以减少复杂度。因此，存在相同的值，不能都预先存入字典中

```python
class solution:
    def twosum(self,nums,target):
        if nums == None or len(nums) < 2:
            return []
        else:
            all = {}
            disparity = target - nums[i]
            if disparity in all:
                return [all[disparity],i]
            else:
                all[nums[i]] = i
        return []
```















