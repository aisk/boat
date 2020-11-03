package boat

func Head[T any](array []T) *T {
	if len(array) == 0 {
		return nil
	}
	return &array[0]
}

func Tail[T any](array []T) []T {
	result := []T{}
	if len(array) == 0 {
		return result
	}
	for i:=1; i<len(array); i++ {
		result = append(result, array[i])
	}
	return result
}

func First[T any](array []T) *T {
	return Head(array)
}

func Last[T any](array []T) *T {
	if len(array) == 0 {
		return nil
	}
	return &array[len(array)-1]
}

func Reverse[T any](array []T) []T {
	reversed := make([]T, len(array))
	for i := range array {
		reversed[i] = array[len(array)-1-i]
	}
	return reversed
}

func Includes[T comparable](array []T, value T) bool {
	for _, a := range array {
		if a == value {
			return true
		}
	}
	return false
}

func Uniq[T comparable](array []T) []T {
	set := make(map[T]struct{})
	for _, a := range array {
		set[a] = struct{}{}
	}
	result := make([]T, len(set))
	i := 0
	for a, _ := range set {
		result[i] = a
		i ++
	}
	return result
}

func Keys[T1 comparable, T2 any](dict map[T1]T2) []T1 {
	keys := make([]T1, len(dict))
	i := 0
	for k, _ := range dict {
		keys[i] = k
		i += 1
	}
	return keys
}

func Values[T1 comparable, T2 any](dict map[T1]T2) []T2 {
	values := make([]T2, len(dict))
	i := 0
	for _, v := range dict {
		values[i] = v
		i += 1
	}
	return values
}
