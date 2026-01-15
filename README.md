# Bright Data의 스크레이핑프록시

[![Promo](https://github.com/bright-kr/Rotating-Residential-Proxies/blob/main/50%25%20off%20promo.png)](https://brightdata.co.kr/proxy-types) 

## Bright Data 소개
Bright Data는 전 세계 20,000명 이상의 고객에게 서비스를 제공하는 수상 경력의 선도적인 프록시 제공업체입니다. 1억 개 이상의 プロキ시 IP, 동급 최고 수준의 기술, 그리고 모든 국가, 도시, 통신사 및 ASN을 타겟팅할 수 있는 역량을 통해 당사의 プロキ시 서비스는 개발자에게 최고의 선택지입니다.

## レジデンシャル프록시
정밀한 타겟팅, 타의 추종을 불허하는 안정성, 그리고 빠른 응답 시간을 제공하도록 설계된 Bright Data의 [스크레이핑프록시](https://brightdata.co.kr/solutions/scraping-proxy)로 원활한 스크레이핑을 경험해 보십시오.

- **72M+ レジデンシャル IP**
- **스티키 및 ローテーティング프록시 세션**
- **99.95% 성공률**
- **HTTP(S) & SOCKS5 지원**
- **지오로케이션 타겟팅(무료)**

## 주요 기능
- **글로벌 커버리지**: [195개 국가](https://brightdata.co.kr/locations)에서 사용 가능한 レジデンシャル프록시를 제공합니다.
- **높은 성공률**: 스크레이핑 프로젝트에서 최대 99.95%의 성공률을 달성합니다.
- **빠른 응답**: 평균 응답 시간은 약 ~0.7초입니다.
- **윤리적 소싱**: 모든 プロキ시는 사용자로부터 명시적 동의를 받아 수집됩니다.
- **무제한 동시 세션**: 제한 없이 운영을 확장할 수 있습니다.

## 요금제
- **종량제(Pay As You Go)**: $8.4/GB, 월 약정이 필요하지 않습니다.
- **월 구독**:
  - **69 GB**: $7.14/GB, $499/월.
  - **158 GB**: $6.3/GB, $999/월.
  - **339 GB**: $5.88/GB, $1999/월.
  - **Enterprise 플랜**: 대규모 요구 사항을 위한 맞춤 솔루션을 제공합니다.

[![Promo](https://github.com/bright-kr/LinkedIn-Scraper/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://brightdata.co.kr/proxy-types) 

## レジデンシャルプロキ시 시작하기
1. **무료 체험 시작**: 신용카드가 필요하지 않습니다.
2. **통합**: API 또는 Control Panel을 사용하여 IP와 구성을 관리합니다.
3. **지원 언어**: Python, Java, C#, Node.js, Shell에 대한 빠른 시작 예제가 제공됩니다.

## 코드 예시

### Python

```python
import sys

# Replace '[your customerID]', 'residential', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 33335);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-residential", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:33335");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-residential", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:33335 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## モバイル프록시
전 세계 수백만 개의 3G, 4G, 5G IP를 제공하는 Bright Data의 [モバイル프록시 네트워크](https://brightdata.co.kr/proxy-types/mobile-proxies)로 실제 모바일 사용자처럼 인터넷에 액세스하십시오.

- **7,000,000+ モバイル IP**
- **3G/4G/5G 모바일 IP**
- **24/7 지원과 함께 99.99% 업타임**
- **지오로케이션 타겟팅(무료)**

## 주요 기능
- **글로벌 범위**: [195개 국가](https://brightdata.co.kr/locations)에 걸친 모바일 IP에 액세스합니다.
- **높은 성공률**: 데이터 수집 및 테스트 작업에서 최대 99.9%의 성공률을 달성합니다.
- **실제 모바일 연결**: 모바일 IP는 실제 네트워크의 실제 디바이스에서 소싱됩니다.
- **무제한 확장**: 동시 연결 세션과 고가용성 인프라로 확장할 수 있습니다.
- **통신사 수준 타겟팅**: 특정 통신사별로 타겟팅하여 심층적이고 정확한 인사이트를 제공합니다.

## 요금제
- **종량제(Pay As You Go)**: 월 약정 없이 $8.4/GB.
- **월 구독**:
  - **69 GB**: $7.14/GB, $499/월 + VAT.
  - **158 GB**: $6.3/GB, $999/월 + VAT.
  - **339 GB**: $5.88/GB, $1999/월 + VAT.
  - **Enterprise 플랜**: 맞춤형 가격과 패키지를 제공합니다.

지금 가입하고 첫 입금에 대해 최대 $500까지 1:1 매칭 혜택을 받으십시오!

## モバイルプロキ시 시작하기
1. **무료 체험 시작**: 신용카드가 필요하지 않습니다.
2. **통합**: API 또는 Bright Data Control Panel을 사용하여 IP와 구성을 관리합니다.
3. **지원 언어**: Python, Java, C#, Node.js, Shell에 대한 빠른 시작 예제가 제공됩니다.

## 코드 예시

### Python

```python
import sys

# Replace '[your customerID]', 'mobile', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-mobile", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-mobile", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell 

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-mobile:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## ISP프록시
ISP로부터 직접 소싱된 IP를 통해 안전하고 안정적이며 고속의 데이터 수집을 수행할 수 있도록, Bright Data의 방대한 [ISP프록시 네트워크](https://brightdata.co.kr/proxy-types/isp-proxies)를 활용하십시오.

- **700,000+ ISP IP**
- 장기 안정성을 제공하는 **スタティック프록시 レジデンシャル IP**
- **99.9% 성공률**
- **HTTP(S) & SOCKS5 지원**
- **국가 단위 타겟팅 무료 제공**

## 주요 기능
- **글로벌 범위**: [여러 국가](https://brightdata.co.kr/locations)에 걸친 ISP IP에 액세스합니다.
- **높은 성공률**: 웹사이트 액세스에서 최대 99.9%의 성공률을 제공합니다.
- **빠르고 안정적임**: 낮은 지연 시간과 안정적인 업타임, 99.99% 네트워크 가용성을 제공합니다.
- **독점 IP 액세스**: 일관된 연결을 위한 전용 IP를 제공합니다.
- **윤리적 소싱**: 모든 ISPプロキ시는 ISP로부터 직접 제공되며 GDPR 및 CCPA를 준수합니다.

## 요금제
- **종량제(Pay As You Go)**: 월 약정 없이 $15/GB로 사용 가능합니다.
- **월 구독 - 공유(Shared)**:
  - **10 IPs**: $1.80/IP, $18/월 + VAT.
  - **100 IPs**: $1.45/IP, $145/월 + VAT.
  - **500 IPs**: $1.40/IP, $700/월 + VAT.
  - **1,000 IPs**: $1.30/IP, $1300/월 + VAT.
  - **Enterprise 플랜**: 대규모 데이터 수집 요구를 위한 맞춤 솔루션을 제공합니다.
 
- **월 구독 - 전용(Dedicated)**:
  - **10 IPs**: $3.50/IP, $35/월 + VAT.
  - **100 IPs**: $2.75/IP, $275/월 + VAT.
  - **500 IPs**: $2.60/IP, $1300/월 + VAT.
  - **1,000 IPs**: $2.50/IP, $2500/월 + VAT.
  - **Enterprise 플랜**: 대규모 데이터 수집 요구를 위한 맞춤 솔루션을 제공합니다.
 
- **월 구독 - Pay/GB**:
  - $12.75/GB, $499/월 + VAT.
  - $11.25/GB, $999/월 + VAT.
  - $10.50/GB, $1999/월 + VAT.
  - **Enterprise 플랜**: 대규모 데이터 수집 요구를 위한 맞춤 솔루션을 제공합니다.


## ISPプロキ시 시작하기
1. **무료 체험 시작**: 신용카드가 필요하지 않습니다.
2. **통합**: Bright Data의 Control Panel 또는 API를 통해 IP와 구성을 관리합니다.
3. **지원 언어**: Python, Java, C#, Node.js, Shell용 빠른 시작 가이드가 제공됩니다.

## 코드 예시

### Python

```python
import sys

# Replace '[your customerID]', 'isp', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-isp", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-isp", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-isp:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## データセンター프록시
신뢰할 수 있는 데이터 수집과 Web스크레이핑을 위해, 압도적인 규모와 속도를 제공하는 Bright Data의 방대한 [データセンター프록시 네트워크](https://brightdata.co.kr/proxy-types/datacenter-proxies)를 활용하십시오.

- **770,000+ データセンター IP**
- **[공유(Shared)](https://brightdata.co.kr/solutions/shared-proxies) 및 [전용(Dedicated)](https://brightdata.co.kr/solutions/dedicated-proxies) IP 옵션**
- **평균 응답 시간 ~0.24초**
- **HTTP(S) & [SOCKS5](https://brightdata.co.kr/solutions/socks5-proxies) 지원**
- **국가 단위 타겟팅 무료 제공**

## 주요 기능
- **글로벌 범위**: [98개 국가](https://brightdata.co.kr/locations)에 걸친 データセンター IP에 액세스합니다.
- **높은 성공률**: 스크레이핑 작업에서 최대 99.9%의 성공률을 달성합니다.
- **빠르고 신뢰할 수 있음**: 99.99% 네트워크 업타임과 빠른 연결 속도를 제공합니다.
- **맞춤형 옵션**: 필요에 따라 공유 또는 전용 IP를 선택할 수 있습니다.
- **무제한 확장**: 제한 없이 동시 연결 세션을 지원합니다.

## 요금제
- **종량제(Pay As You Go)**: 월 약정 없이 $0.6/GB로 이용 가능합니다.
- **월 구독 - 공유(Shared)**:
  - **10 IPs**: $1.40/IP, $14/월 + VAT.
  - **100 IPs**: $1.00/IP, $100/월 + VAT.
  - **500 IPs**: $0.95/IP, $475/월 + VAT.
  - **1,000 IPs**: $0.90/IP, $900/월 + VAT.
  - **Enterprise 플랜**: 대규모 데이터 수집을 위한 맞춤 솔루션을 제공합니다.

- **월 구독 - 전용(Dedicated)**:
  - **10 IPs**: $2.20/IP, $22/월 + VAT.
  - **100 IPs**: $1.70/IP, $170/월 + VAT.
  - **500 IPs**: $1.50/IP, $750/월 + VAT.
  - **1,000 IPs**: $1.30/IP, $1300/월 + VAT.
  - **Enterprise 플랜**: 대규모 데이터 수집을 위한 맞춤 솔루션을 제공합니다.


- **월 구독 - Pay/GB**:
  - $0.51/GB, $499/월 + VAT.
  - $0.45/GB, $999/월 + VAT.
  - $0.42/GB, $1999/월 + VAT.
  - **Enterprise 플랜**: 대규모 데이터 수집을 위한 맞춤 솔루션을 제공합니다.

가입하고 첫 입금에 대해 최대 $500까지 1:1 매칭 혜택을 받으십시오!

## データセンタープロキ시 시작하기
1. **무료 체험 시작**: 신용카드가 필요하지 않습니다.
2. **통합**: API 또는 Bright Data Control Panel로 IP와 구성을 관리합니다.
3. **지원 언어**: Python, Java, C#, Node.js, Shell용 빠른 시작 가이드를 제공합니다.

## 코드 예시

### Python

```python
import sys

# Replace '[your customerID]', 'datacenter', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-datacenter", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-datacenter", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
    })
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```
### 지금 [Bright Data](https://brightdata.co.kr)에 참여하여 업계 리더인 이유를 확인해 보십시오. 