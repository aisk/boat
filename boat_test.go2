package boat

import "testing"

func TestHead(t *testing.T) {
	if *Head([]string{"foo", "bar"}) != "foo" {
		t.Fail()
	}
}

func TestTail(t *testing.T) {
	result := Tail([]string{"foo", "bar", "baz"})
	if len(result) != 2 {
		t.Fail()
	}
	if result[0] != "bar" || result[1] != "baz" {
		t.Fail()
	}

	result = Tail([]string{})
	if len(result) != 0 {
		t.Fail()
	}
}

func TestLast(t *testing.T) {
	if *Last([]string{"foo", "bar"}) != "bar" {
		t.Fail()
	}
}

func TestReverse(t *testing.T) {
	reversed := Reverse([]string{"foo", "bar", "baz"})
	if reversed[0] != "baz" {
		t.Fail()
	}
	if reversed[1] != "bar" {
		t.Fail()
	}
	if reversed[2] != "foo" {
		t.Fail()
	}
}

func TestIncludes(t *testing.T) {
	if !Includes([]string{"foo", "bar"}, "foo") {
		t.Fail()
	}
	if Includes([]string{"foo", "bar"}, "baz") {
		t.Fail()
	}
}

func TestUniq(t *testing.T) {
	result := Uniq([]string{"foo", "bar", "foo"})
	if len(result) != 2 {
		t.Fail()
	}
}

func TestKeys(t *testing.T) {
	keys := Keys(map[string]int{"foo": 1, "bar": 2, "baz": 3})
	if len(keys) != 3 || keys[0] != "foo" || keys[1] != "bar" || keys[2] != "baz" {
		t.Fail()
	}
}

func TestValues(t *testing.T) {
	values := Values(map[string]int{"foo": 1, "bar": 2, "baz": 3})
	if len(values) != 3 || values[0] != 1 || values[1] != 2 || values[2] != 3 {
		t.Fail()
	}
}
