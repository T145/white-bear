<div align="center">
  <img src=".github/images/logo.jpg"
       width="600"
       alt="logo"
       longdesc="https://github.com/T145/white-bear/master/README.md" />
  <h3>🔱 Delve | 🪄 Demystify | 🛑 Deny</h3>
  <hr>
  <p>DoH, DoT, DNSCrypt, &amp; DoQ provider whitelists and blacklists.</p>
  <hr>
  <img src="https://badges.pufler.dev/updated/T145/white-bear"
       alt="last_updated"
       longdesc="https://pufler.dev/git-badges/"
       crossorigin="anonymous"
       referrerpolicy="no-referrer" />
  <img src="https://badges.pufler.dev/visits/T145/white-bear"
       alt="visits"
       longdesc="https://pufler.dev/git-badges/"
       crossorigin="anonymous"
       referrerpolicy="no-referrer" />
  <a href="https://github.com/T145/white-bear/commits/master.atom">
    <img src="https://img.shields.io/static/v1?logo=rss&label=rss&message=feed&color=FFA500"
        alt="release"
        longdesc="https://github.com/badges/shields/"
        crossorigin="anonymous"
        referrerpolicy="no-referrer" />
  </a>
</div>

## 🖋️ Details

> There may be discovered exceptions and this section may be modified in the future.

Similar projects that this one could be considered a spiritual successor to are as follows:

- [dohservers](https://github.com/oneoffdallas/dohservers)
- [TheGreatWall](https://github.com/Sekhan/TheGreatWall)

[TheGreatWall's description](https://github.com/Sekhan/TheGreatWall#what-is-dns-over-https-doh-=) and [AdGuard's article on DoQ](https://adguard.com/en/blog/dns-over-quic.html) provide great overviews for this topic. When deciding whether or not to block a specific encrypted DNS provider domain, it's important to read their policies. Some have actually engineered services that focus on privacy and value the encryption provided by the technology, while others use it to harvest more information on their users.

Regardless of policy, however, it's safe to assume that *all* DoH (DNS-over-HTTPS) providers should be blocked due to [security considerations](https://datatracker.ietf.org/doc/html/rfc8484#section-9). This stems from the fact that HTTPS is **not** transport layer protocol.

Regarding other services, those that ultimately support privacy will be whitelisted, and the latter variants will be blocked.

## References

- https://dnsprivacy.org/test_servers/#stubby-configuration
  - https://raw.githubusercontent.com/getdnsapi/stubby/develop/stubby.yml.example
- https://github.com/curl/curl/wiki/DNS-over-HTTPS#publicly-available-servers
