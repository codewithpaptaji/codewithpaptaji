from switchlang import switch

def handle_case(value):
    with switch(value) as s:
        s.case(1, handle_case1)
        s.case(2, handle_case2)
        s.case(3, handle_case3)
        s.default(default_action)()

def handle_case1():
    # Code for case 1
    pass

def handle_case2():
    # Code for case 2
    pass

def handle_case3():
    # Code for case 3
    pass

def default_action():
    # Code for other cases
    pass
