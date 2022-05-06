
```

empty = null
boolean = true
string_no_escape = 'ha'
string_simple = "hello"


string_complex = """
kill
all
humans
"""


// possibly problamatic def slow
timestamp = 2022-05-06T01:23:39+00:00
uuid = e18630ee-42d0-4a56-bc93-d651679402b9
email = John.Doe@example.com

// ambigous
spdx = (MIT or CC0)
expression = (defun foo (a b c d) (+ a b c d))

// can't have hostname true, false, or null
hostname = www.google.com


uri = tel:+1-816-555-1212
i64 = 42
f64 = 1.2e3
bytes = 0xFFFFFFFF
regex = /^([\w\.%\+\-]+)@([\w\-]+\.)+([\w]{2,})$/i

pattern = $"hello {{assholes}}"
argument = $arg
default = ${arg:-"fuckyou"}


semver = 1.0.0-alpha+001
percentage = 32.3%
quantity = %32 USD%
quantity = %USD 32%
quantity = %32 m^-2%
array = [1.0 42 1.2e3]
object = {"COPY":{"attributes":{"chown":"55:mygroup"},"value":["files*","/somedir/"]}}

ipv6 = fe80::1ff:fe23:4567:890a
ipv4 = 169.254.255.255
socket = [fe80::1ff:fe23:4567:890a%25eth0]:8443
socket = 0.0.0.0:8888
socket = google.com:8888
hostname = www.google.com

color = rgb(1, 2, 3)
color = #deadbeaf

code_line = `fuck this shit`
code = ```python
whatever
```

label &label = "idk something"
referance = *symbol

nested.assignment[].is[okay] = 3


```


```

```
[ hello ] = [ "hello" ]

[hello] format 1.3.4
    world { big true dead false }
    you.are really.nice count [ { [fuck] you 1 } 2 3]
[bye]

= 
{ "hello" : { "world" : false, {"you" : { "are" : "really.nice" }} }, "bye" : {} }



```




label = dns_label | string

assign = key assign_sym? value
assign_sym = "=" | ":"



```dockerfile
RUN /bin/bash -c 'source $HOME/.bashrc;\
echo $HOME'

RUN ["/bin/bash", "-c", "echo hello"]


REGEX /ab+c/

ADD \
    valid = false \
    integer = 32 \
    now = 2022-05-06T01:23:39+00:00 \
    void = null \
    patern = /ab+c/

COPY --chown=55:mygroup files* /somedir/
```

```toml
my = 1
[all]
cops : 'basterds'
nest = {
    [fuck]
    this = 'shit'
}
```



```json
[
  {
    "RUN": "/bin/bash -c 'source $HOME/.bashrc;\necho $HOME'"
  },
  {
    "RUN": [
      "/bin/bash",
      "-c",
      "echo hello"
    ]
  },
  {
      "COPY" : {
          "attributes": {
            "chown" : "55:mygroup"
          },
          "value" : [ "files*", "/somedir/" ]
      }
  },
  {
      "REGEX" : "/ab+c/"
  }
]
```