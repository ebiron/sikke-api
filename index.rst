# Cüzdan

## Bakiye Sorgulama
<table>
<tr>
            <th align="right">GET</th>
            <td colspan="2"><code>/wallet/balance/{sikke_cuzdan_numarası}</code></td>
        </tr>
        <tr>
            <th align="right">REQUEST</th>
            <td colspan="2"><a href="https://api.sikke.network/v1/wallet/balance/SKK1N5WHL2m6WcfqF29Uj19nKvUaRwpUeg1Fr">https://api.sikke.network/v1/wallet/balance/SKK1N5W...</a></td>
        </tr>
        <tr>
            <th align="right" valign="top"> RESPONSE </th>
            <td align="left" valign="top" width="50%">
<pre>{
    "balance":0
}</pre></td>
<td valign="top" width="50%">
<p><code>balance</code> <i>(double)</i> :  Kese bakiyesi </p>
</td></tr>
</table>


## Kese Oluşturma

Sikke platformunda yeni bir kese oluşturmak için aşağıdaki metod kullanılabilir. Oluşturulan Kesenin Private Key'i hiç bir yere kayıt edilmez.

<table>
<tr>
            <th align="right">GET</th>
            <td colspan="2"><code>/wallet/generate_wallet</code></td>
        </tr>
        <tr>
            <th align="right">REQUEST</th>
            <td colspan="2">https://api.sikke.network/v1/wallet/generate_wallet</td>
        </tr>
        <tr>
            <th align="right" valign="top"> RESPONSE </th>
            <td align="left" valign="top" width="50%">
<pre>{
	"status": "success",
	"wallet": {
		"address": "SKK12mewJbFDu...",
		"private_key": "94ijfgLABB21ANgGE...",
		"public_key": "3DL69o6RYTg...."
	}
}</pre></td>
<td valign="top" width="50%">
<p><code>status</code> [success/error] <i>(string)</i> :  API Cevap</p>
<p><code>address</code> <i>(string)</i> :  Kese Numarası</p>
<p><code>private_key</code> <i>(string)</i> :  Kese Private Key</p>
<p><code>public_key</code> <i>(string)</i> :  Kese Public Key</p>
</td></tr>
</table>

# TX (Transfer İşlemleri)

Sikke platformunda gerçekleşmiş olan bir işlemin detaylarına ulaşmak için aşağıdaki metod kullanılabilir.

<table>
    <col width="25%">
    <col width="75%">
    <thead>
        <tr>
            <th> GET </th>
            <th align="left">/v1/tx/{islem_numarasi}</th>
        </tr>
    </thead>
</table>


<table>
    <col width="25%">
    <col width="50%">
    <col width="25%">
    <thead>
        <tr>
            <th>URL Parametreleri</th>
            <th>Açıklama</th>
            <th>Veritipi</th>
        </tr>
    </thead>
    <tbody>
        <tr align="center">
            <td> w_pub_key </td>
            <td> is_hidden değeri 1 olan işlemlerde tüm bilgilere ulaşmak için cüzdanın public key numarası girilmelidir. </td>
            <td>String</td>
        </tr>
    </tbody>
</table>


Örnek Kullanım: `api.sikke.network/v1/tx/a81f10607116321fc3ec0290efe2f233cdecd13eda192f9147cd372b03593a79?w_pub_key`


## İşlem Listeleri

Sikke platformunda gerçekleşen anlık işlemlerin detaylarına ulaşmak için bu aşağıdaki metod kullanılabilir.

<table>
    <col width="25%">
    <col width="75%">
    <thead>
        <tr>
            <th> GET </th>
            <th align="left">/v1/tx</th>
        </tr>
    </thead>
</table>



Örnek Kullanım: `api.sikke.network/v1/tx?user_id&wallet&asset&type&subtype=&status&skip=0&limit=100&sort=desc&seq_gt=&wallets=&w_pub_key&from_date=&to_date=&get_my_tx=` 

<table>
    <col width="25%">
    <col width="50%">
    <col width="25%">
    <thead>
        <tr>
            <th>URL Parametreleri</th>
            <th>Açıklama</th>
            <th>Veritipi</th>
        </tr>
    </thead>
    <tbody>
        <tr align="center">
            <td> user_id </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> wallet </td>
            <td>Cüzdan Numarası</td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> asset </td>
            <td>  </td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> type </td>
            <td> </td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> subtype </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> status </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> skip </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> limit </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> sort </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> seq_gt </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> wallets </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> w_pub_key </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> from_date </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> to_date </td>
            <td></td>
            <td>String</td>
        </tr>
        <tr align="center">
            <td> get_my_tx </td>
            <td></td>
            <td>String</td>
        </tr>
    </tbody>
</table>

