BPJS Kesehatan Indonesia
PHP package to access BPJS Kesehatan API This package is a wrapper of BPJS VClaim Web Service V2

Installation 🔥
composer require bridging/bpjs

Example Usage :
//use your own bpjs config
$vclaim_conf = [
    'cons_id' => '123456',
    'secret_key' => '123456',
    'base_url' => 'https://dvlp.bpjs-kesehatan.go.id',
    'service_name' => 'vclaim-rest'
];

// use Referensi service
$referensi = new Bridging\Bpjs\VClaim\Referensi($vclaim_conf);
var_dump($referensi->diagnosa('A00'));

$peserta = new Bridging\Bpjs\VClaim\Peserta($vclaim_conf);
var_dump($peserta->getByNoKartu('123456789','2018-09-16'));
Supported Services (WIP) 🚀
 Referensi
 Peserta
 SEP
 Rujukan
 Lembar Pengajuan Klaim
 Monitoring
 PRB
 Rencana Kontrol
 Aplicare
REFERENSI REST 📘
Vclaim V2.0 Trust Mark: https://dvlp.bpjs-kesehatan.go.id:8888/trust-mark/portal.html
Pcare v3.0: https://new-api.bpjs-kesehatan.go.id/pcare-rest-v3.0/
BASED ON & CREDIT THANKS 👍
https://github.com/nsulistiyawan/bpjs
