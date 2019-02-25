---
title: "mkdir"
date: 2019-02-14T10:04:59+09:00
categories:
- commands
- mkdir
tags:
- rust
keywords:
- coding challenge
thumbnailImage: https://1.bp.blogspot.com/-hVGiemkjg58/V5NECYgvcxI/AAAAAAAA8gk/aj0H6AbBIV4XOIdF964KDN48oNCsy0qjgCLcB/s800/ha_kenkou_oldman.png
---

# mkdir - *make directories*

This time, I write unix `mkdir` command with rust.

*Code on my GitHub repo:*
<div class="iframely-embed"><div class="iframely-responsive" style="height: 168px; padding-bottom: 0;"><a href="https://github.com/kHigasa/rustcli/blob/master/mkdir/mkdir/src/main.rs" data-iframely-url="//cdn.iframe.ly/8tLVzR6"></a></div></div><script async src="//cdn.iframe.ly/embed.js" charset="utf-8"></script>

*Live coding demo on my YouTube channel:*
{{< youtube d2k3FXUmH7I>}}

## Tasks

- Make directories -> use `std::fs` module `create_dir` function
- Parse command line option -> use `getopts` crate
- Set permission -> use `std::os::unix::fs` module

### Pseudo code

```
options.match
    m => mkdir; set permission;
    p => mkdir recursively;
    h => print usage;
    _ => if !args.is_empty()
             mkdir;
         else
             print usage;
```

### Tips

Use `getopts` crate to parse option easily :)

#### References

- [Module std::fs](https://doc.rust-lang.org/std/fs/index.html)
- [Crate getopts](https://docs.rs/getopts/)
- [mkdir: Make directories](https://www.gnu.org/software/coreutils/mkdir)

