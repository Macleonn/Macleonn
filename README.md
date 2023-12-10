#include <iostream>

int solution(int number) {
  int sum = 0;
  for (int i = 1; i < number; ++i) {
    if (i % 3 == 0 || i % 5 == 0) {
      sum += i;
    }
  }
  return sum;
}

int main() {
  std::cout << "Sum of multiples of 3 or 5 below 10: " << solution(10) << std::endl;
  std::cout << "Sum of multiples of 3 or 5 below 20: " << solution(20) << std::endl;
  std::cout << "Sum of multiples of 3 or 5 below 30: " << solution(30) << std::endl;
  return 0;
}
