# shareit-cwe-789 - Uncontrolled Memory Allocation
*CVE-2019-14941<br/>
SHAREit v4.0.6.177's unsecured channel for Windows does not check the body length from the received packet header. The body length is used to allocate memory for the expected data to be received. This could lead to resource exhaustion with the limitation of theoretically being able to allocate a maximum 2 GB of memory.<br/><br/> 
*CVE-2019-15234<br/>
SHAREit v4.0.6.177's secured channel for Windows does not check the full message length from the received packet header. The full message length is used to allocate memory for the expected data to be received. This could lead to resource exhaustion with the limitation of theoretically being able to allocate a maximum 2 GB of memory.