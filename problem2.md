
function dot_product(v1, v2, n):
    ps = 0  
    for i = 0 to n - 1:
        ps = ps + v1[i] * v2[i]  
    end for
    return ps  
end function


procedure check_orthogonality(vectors1, vectors2, n, length_of_vector):
    for i = 0 to n - 1:
        ps = dot_product(vectors1[i], vectors2[i], length_of_vector)
        if ps != 0:
            print("Vectors", i, "are not orthogonal.")
        else:
            print("Vectors", i, "are orthogonal.")
    end for
end procedure


vectors1 = [[3, 1, 7], [1, 2, 3], [4, 5, 6]]
vectors2 = [[2, 4, 1], [3, 0, -1], [4, 3, 2]]
n = 3
length_of_vector = 3

check_orthogonality(vectors1, vectors2, n, length_of_vector)
