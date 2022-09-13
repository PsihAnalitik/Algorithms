class Solution {
public:
    int firstBadVersion(int n) {
      int left = 0;
      int right = n;
      int current = 0;
      if(n < 2) return n;
      while(left <= right){
          current = (right - left)/2 + left;
          if(isBadVersion(current)){

              if(!isBadVersion(current -1)) return current;
              else {
                  right = current -1;
              }


          }
          if(!isBadVersion(current)){
              left = current + 1;
          }
      }
    
    return current;
    }
};
