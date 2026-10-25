
Access control represents controlling what resources users have access based on different parameters like privileges. For it to work there needs to be a sound authentication a good session management. Covering such a wide range of actions there also exist a lot of way for access control to be broken.

## Absent Checks

1.  **[Unprotected admin functionality](https://portswigger.net/web-security/access-control/lab-unprotected-admin-functionality)** -> In this lab we had no active access control, the defense is based on user lack of knowledge. By looking at app's `robots.txt`  we see the name of the admin page which is accessible by all users.
2. **[Unprotected admin functionality with unpredictable URL](https://portswigger.net/web-security/access-control/lab-unprotected-admin-functionality-with-unpredictable-url)** -> Here its the same situation as the one above, but the name of the admin page is non-standard and not present in `robots.txt`. Looking at the DevTools in the Debugg window we see some Java Script which loads elements based on role. In the code we will see leaked the name of the admin page, under the check isAdmin. 

## Checks on attacker controlled values 

1. **[User role controlled by request parameter](https://portswigger.net/web-security/access-control/lab-user-role-controlled-by-request-parameter)** ->
2.  **[User ID controlled by request parameter](https://portswigger.net/web-security/access-control/lab-user-id-controlled-by-request-parameter)** ->
3. **[User ID controlled by request parameter, with unpredictable user IDs](https://portswigger.net/web-security/access-control/lab-user-id-controlled-by-request-parameter-with-unpredictable-user-ids)** ->
4. **[User ID controlled by request parameter with data leakage in redirect](https://portswigger.net/web-security/access-control/lab-user-id-controlled-by-request-parameter-with-data-leakage-in-redirect)** ->
5. **[User ID controlled by request parameter with password disclosure](https://portswigger.net/web-security/access-control/lab-user-id-controlled-by-request-parameter-with-password-disclosure)** ->

## Obstacles



## Checks at the wrong layer

1. **URL-based access control** -> 