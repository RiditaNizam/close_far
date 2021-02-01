# close_far
CodingBat Python Logic-2

Given three ints, a b c, return True if one of b or c is "close" (differing from a by at most 1), while the other is "far", differing from both other values by 2 or more. Note: abs(num) computes the absolute value of a number.


def close_far(a, b, c):

    #b is close and c is far
    if abs(a-b) <= 1 and (abs(a-c) >= 2 and abs(b-c) >= 2):
      return True
    #c is close and b is far
    if abs(a-c) <= 1 and (abs(a-b) >= 2 and abs(b-c) >= 2):
      return True
    else:
      return False
