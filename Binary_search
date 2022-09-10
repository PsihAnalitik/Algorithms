#include <iostream>
#include <vector>
using std::vector;

class BinaryTree{

    public:
        int search(vector<int> &nums, int target){
            unsigned int left = 0;
            unsigned int right = nums.size();
            if(nums.size() == 1){
                if(target == nums[0]){
                    return 0;
                }
                return -1;
            }
            unsigned int curElement = nums.size()/2;
            while(left <= right){
                if(target > nums[curElement]){
                    if(curElement < nums.size()){
                        left = curElement+1;
                    }
                    else return -1;
                    curElement = (left + right)/2;
                }
                if(target < nums[curElement]){
                    if(curElement > 0){
                        right = curElement-1;
                    }
                    else return -1;
                    curElement = (left + right)/2;
                }
                if(target == nums[curElement]) return (int)curElement;
            }
            return -1;

        }

};

int main() {
    using namespace std;
    vector<int> vec;
    int k;
    cin >> k;
    for(int i=0; i<k;i++){
        int el;
        cin >> el;
        vec.push_back(el);
    }
    int target;
    cin >> target;
    BinaryTree tree;
    cout << tree.search(vec,target);
    return 0;
}
