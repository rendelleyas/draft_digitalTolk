## Code

What makes it amazing code?
- Readability
    : personally, for me the code is readable


What makes it terrible code?
 - Ununiformed variable naming
    : There are multiple format of variable naming. like '$consumer_type', '$completeddate', and '$adminSenderEmail'
    : Consistency allows others to more easily understand your code.
 - Unecessary variables
    : there are declared variable who are not utilized
    : can confused why is it existing, whats its purpose

How would you have done it
 - Ununiformed variable naming
    : Personaly I prefer camelCase its looks shorter than snake_case with additional '_'.
    : Team should have a code guidelines  - list all the  recommended styles and practices (variable and function namings)
 - Uncomplex condition
    : on simple condition its better to use ternary operator than else if
    ```
        From: 
            if (isset($data['distance']) && $data['distance'] != "") {
                $distance = $data['distance'];
            } else {
                $distance = "";
            }
        =========
        To: 
            $distance = isset($data['distance']) && $data['distance'] != ""? $data['distance'] : "";
    ```
 - Unecessary variables
    : remove unecessary or unutilized variables
    ```
        From:
            $response = $this->repository->getUsersJobsHistory($user_id, $request);
            return response($response);
        =========
        To:
            return response($this->repository->getUsersJobsHistory($user_id, $request));

    ```
 


Thoughts on formatting, structure, logic and etc.
 - 

Suggestion



=====
