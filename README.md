# ipdb-java
用于解析离线数据库


# 代码示例
## 地级市精度库
<pre>
        try {
            // City类可用于IPDB格式的IPv4/IPv6定制版本
            City db = new City("/path/to/ipiptest.ipdb");
            
            // db.find(address, language) 返回索引数组
            System.out.println(Arrays.toString(db.find("1.1.1.1", "CN")));

            // db.findInfo(address, language) 返回 CityInfo 对象
            CityInfo info = db.findInfo("118.28.1.1", "CN");
            System.out.println(info);

        } catch (Exception e) {
            e.printStackTrace();
        }
</pre>

<p>IP地址位置数据由<a href="https://www.cz88.net">纯真CZ88</a>提供支持</p>
