def merge(self, nums1, m, nums2, n) -> list:
    """
    :type nums1: List[int], length m+n - non-descending
    :type m: int
    :type nums2: List[int], length n - non-descending
    :type n: int
    :rtype: None Do not return anything, modify nums1 in-place instead.
    """

    for j in range(n):
            
        if m+j == 0:

            nums1.insert(0, nums2[j])
            nums1.pop(-1)
        
        else:
        
            for i in range(m+j+1):

                if nums2[j] <= nums1[i]:

                    nums1.insert(i, nums2[j])
                    nums1.pop(-1)
                    break
            
                elif i < m+j and nums1[i+1] < nums1[i]:
                    
                    nums1.insert(i+1, nums2[j])
                    nums1.pop(-1)
                    break
            
                elif i == m+j:
                    
                    nums1.insert(i, nums2[j])
                    nums1.pop(-1)
                    break
  return nums1
