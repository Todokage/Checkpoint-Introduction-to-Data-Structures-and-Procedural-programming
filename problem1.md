function sum_of_distinct_elements(set1, set2):
    sum = 0

    
    for i from 0 to length(set1) - 1:
        if set1[i] is not in set2:
            sum = sum + set1[i]

    
    for j from 0 to length(set2) - 1:
        if set2[j] is not in set1:
            sum = sum + set2[j]

    return sum
