<div align="center">
  <img src=".github/images/logo.png"
       width="600"
       alt="logo"
       longdesc="https://github.com/T145/white-bear/master/README.md" />
  <h3>🏊🏿‍♀️ Delve | 📸 Demystify | 🛑 Deny</h3>
  <hr>
  <p><a href="https://en.wikipedia.org/wiki/DNS_over_HTTPS">DoH</a>, <a href="https://en.wikipedia.org/wiki/DNS_over_TLS">DoT</a>, <a href="https://dnscrypt.info/">DNSCrypt</a>, &amp; <a href="https://adguard.com/en/blog/dns-over-quic.html">DoQ</a> provider whitelists and blacklists.</p>
  <p>A spiritual successor to <a href="https://github.com/oneoffdallas/dohservers">dohservers</a> and <a href="https://github.com/Sekhan/TheGreatWall">TheGreatWall</a>.</p>
  <hr>
  <img src="https://badges.pufler.dev/updated/T145/white-bear"1
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

> There may be discovered exceptions and this section could be modified in the future.

[TheGreatWall's description](https://github.com/Sekhan/TheGreatWall#what-is-dns-over-https-doh-=) and [AdGuard's article on DoQ](https://adguard.com/en/blog/dns-over-quic.html) provide great overviews for DNS blacklisting and whitelisting.

When deciding whether or not to block a specific encrypted DNS provider domain, it's important to read their policies. Some have actually engineered services that focus on privacy and value the encryption provided by the technology, while others use it to harvest more information on their users.

Regardless of policy, however, it's safe to assume that *all* DoH (DNS-over-HTTPS) providers should be blocked due to [security considerations](https://datatracker.ietf.org/doc/html/rfc8484#section-9). This stems from the fact that HTTPS is **not** a transport layer protocol.

It's recommended to use `data/v2/doh.csv` as a blacklist and all other lists as a whitelist.

### List References

- https://dnsprivacy.org/test_servers/#stubby-configuration
  - https://raw.githubusercontent.com/getdnsapi/stubby/develop/stubby.yml.example
- https://github.com/curl/curl/wiki/DNS-over-HTTPS#publicly-available-servers
- https://kb.adguard.com/en/general/dns-providers

### TODO

- https://github.com/bebasid/bebasdns
- https://github.com/pengelana/blocklist/wiki/DNS-over-HTTPS-(DoH)
