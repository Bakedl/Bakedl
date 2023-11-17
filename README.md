
def fibonacci_sequence(n):
    a, b = 0, 1
    sequence = []
    for _ in range(n):
        a, b = b, a + b
        sequence.append(a)

    return sequence

def print_fibonacci_triangle(sequence):
    print('\n')
    print('o'.center(30))
    print('|'.center(30))
    print('|'.center(30))

    for num in sequence:
        print(' '.join([i for i in str(num)]).center(30))

    print(('=' * 25).center(30))
    print(('B U R J  K H A L I F A').center(29))
    print(('=' * 25).center(30))

def print_burj_khalifa_info(length, breadth, height, floors):
    print(f'\nLength: {length} meters')
    print(f'Breadth: {breadth} meters')
    print(f'Height: {height} meters')
    print(f'Floors: {floors}')
burj_length = 828
burj_breadth = 144
burj_height = 828
burj_floors = 163
num_fibonacci_numbers = 49
fibonacci_sequence_result = fibonacci_sequence(num_fibonacci_numbers)
print_fibonacci_triangle(fibonacci_sequence_result)
print_burj_khalifa_info(burj_length, burj_breadth, burj_height, burj_floors)
