import random

HEAD = 1
TAIL = 2
NB_TRIES = 10

#true if there is at least one HEAD, false if not
def do_exp(p_nb_tries):
    head_count = 0
    temp_result = 0
    for i in range(1, p_nb_tries + 1):
        temp_result = random.randrange(HEAD, TAIL + 1)
        if temp_result == HEAD:
            head_count += 1

    return (head_count != 0)

def repeat_exp(p_nb_exp, p_nb_tries):
    ret_count = 0
    for i in range(1, p_nb_exp + 1):
        if (do_exp(p_nb_tries) == True):
            ret_count += 1

    return (ret_count / p_nb_exp)


def get_sum(p_n):
    ret = 0
    for i in range(1, p_n + 1):
        ret += 0.5**i

    return (ret)

print(repeat_exp(1000, NB_TRIES))
print(get_sum(NB_TRIES))
