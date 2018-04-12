# Aplikasi Fakultas Ilmu Komputer

Base url: `https://apap-fasilkom.herokuapp.com`

API List:
* [api/mahasiswa/viewall](#apimahasiswaviewall)
* [api/mahasiswa/view/id/[id_mahasiswa]](#apimahasiswaviewidid_mahasiswa)
* [api/mahasiswa/view/npm/[npm]](#apimahasiswaviewnpmnpm)
* [api/matkul/viewall](#apimatkulviewall)
* [api/matkul/view/id/[id_matkul]](#apimakulviewidid_matkul)
* [api/matkul/view/kode/[kode_matkul]](#apimatkulviewkodekode_matkul)
* [api/dosen/viewall](#apimahasiswaviewall)
* [api/dosen/view/id/[id_dosen]](#apidosenviewidid_dosen)
* [api/dosen/view/nip/[nip]](#apidosenviewnipnip)
* [api/staf/viewall](#apimahasiswaviewall)
* [api/staf/view/id/[id_staf]](#apimahasiswaviewidid_mahasiswa)
* [api/staf/view/nip/[nip]](#apistafviewnipnip)

## api/mahasiswa/viewAll

Mengembalikan daftar seluruh mahasiswa

**URL** : `/api/mahasiswa/viewall`

**Method** : `GET`

### Response

**Contoh Request**: [/api/mahasiswa/viewall](https://apap-fasilkom.herokuapp.com/api/mahasiswa/viewall)

```json
[
  {
    "id": 3,
    "npm": "1506721775",
    "nama": "Sosro Liang",
    "mataKuliahList": [
      {
        "id": 12,
        "kode_matkul": "CSIE604180",
        "nama_matkul": "Manajemen Pengetahuan"
      },
      {
        "id": 14,
        "kode_matkul": "UIST601014",
        "nama_matkul": "Matematika Dasar 1"
      },
      {
        "id": 11,
        "kode_matkul": "CSIE604378",
        "nama_matkul": "Manajemen Layanan TI"
      },
      {
        "id": 15,
        "kode_matkul": "CSGE601010",
        "nama_matkul": "Matematika Diskret 1"
      },
      {
        "id": 13,
        "kode_matkul": "CSIE604165",
        "nama_matkul": "Manajemen Rantai Suplai"
      }
    ]
  },
  {
    "id": 4,
    "npm": "1506721781",
    "nama": "Tjahjana Tao",
    "mataKuliahList": [
      {
        "id": 19,
        "kode_matkul": "CSIM602266",
        "nama_matkul": "Sistem Informasi Akuntansi Keuangan"
      },
      {
        "id": 16,
        "kode_matkul": "CSGE603291",
        "nama_matkul": "Metodologi Penelitian & Penulisan Ilmiah"
      },
      {
        "id": 18,
        "kode_matkul": "CSIM603229",
        "nama_matkul": "Proyek Pengembangan Sistem Informasi"
      },
      {
        "id": 20,
        "kode_matkul": "CSIM602262",
        "nama_matkul": "Sistem-Sistem Perusahaan"
      },
      {
        "id": 17,
        "kode_matkul": "CSGE602022",
        "nama_matkul": "Perancangan & Pemrograman Web"
      }
    ]
  }
]
```

## api/mahasiswa/view/id/[id_mahasiswa]

Mengembalikan object seorang mahasiswa dengan menggunakan ID mahasiswa

**URL** : `/api/mahasiswa/view/id/[id_mahasiswa]`

**Method** : `GET`

### Response
**Contoh Request**: [/api/mahasiswa/view/id/1](https://apap-fasilkom.herokuapp.com/api/mahasiswa/view/id/1)

```json
{
  "id": 1,
  "npm": "1506721756",
  "nama": "Abishai Gea",
  "mataKuliahList": [
    {
      "id": 3,
      "kode_matkul": "CSIE604284",
      "nama_matkul": "Analitika Media Sosial"
    },
    {
      "id": 4,
      "kode_matkul": "CSIM601251",
      "nama_matkul": "Dasar-Dasar Arsitektur Komputer"
    },
    {
      "id": 5,
      "kode_matkul": "CSIE604160",
      "nama_matkul": "E-Dagang"
    },
    {
      "id": 2,
      "kode_matkul": "CSGE602012",
      "nama_matkul": "Aljabar Linier"
    },
    {
      "id": 1,
      "kode_matkul": "CSIE604274",
      "nama_matkul": "Administrasi Sistem"
    }
  ]
}
```

## api/mahasiswa/view/npm/[npm]

Mengembalikan object seorang mahasiswa dengan menggunakan npm mahasiswa

**URL** : `/api/mahasiswa/view/npm/[npm]`

**Method** : `GET`

### Response

**Contoh Request**: [/api/mahasiswa/view/npm/1506721756](https://apap-fasilkom.herokuapp.com/api/mahasiswa/view/npm/1506721756)

```json
{
  "id": 1,
  "npm": "1506721756",
  "nama": "Abishai Gea",
  "mataKuliahList": [
    {
      "id": 3,
      "kode_matkul": "CSIE604284",
      "nama_matkul": "Analitika Media Sosial"
    },
    {
      "id": 4,
      "kode_matkul": "CSIM601251",
      "nama_matkul": "Dasar-Dasar Arsitektur Komputer"
    },
    {
      "id": 5,
      "kode_matkul": "CSIE604160",
      "nama_matkul": "E-Dagang"
    },
    {
      "id": 2,
      "kode_matkul": "CSGE602012",
      "nama_matkul": "Aljabar Linier"
    },
    {
      "id": 1,
      "kode_matkul": "CSIE604274",
      "nama_matkul": "Administrasi Sistem"
    }
  ]
}
```

## api/matkul/viewAll

Mengembalikan daftar seluruh mata kuliah

**URL** : `/api/matkul/viewall`

**Method** : `GET`

### Response

**Contoh Request**: [/api/matkul/viewall](https://apap-fasilkom.herokuapp.com/api/matkul/viewall)

```json
[
  {
    "id": 1,
    "kode_matkul": "CSIE604274",
    "nama_matkul": "Administrasi Sistem",
    "dosenList": [
        {
          "id": 1,
          "nip": "1290578781",
          "nama": "Heri Kurniawan S.Kom., M.Kom."
        }
      ]
    },
    {
      "id": 2,
      "kode_matkul": "CSGE602012",
      "nama_matkul": "Aljabar Linier",
      "dosenList": [
        {
          "id": 2,
          "nip": "1290578783",
          "nama": "Dr. Dra. Kasiyah M.Sc"
        }
      ]
    }
  }
]
```

## api/matkul/view/id/[id_matkul]

Mengembalikan object sebuah mata kuliah dengan menggunakan ID mata kuliah

**URL** : `/api/matkul/view/id/[id_matkul]`

**Method** : `GET`

### Response
**Contoh Request**: [/api/matkul/view/id/1](https://apap-fasilkom.herokuapp.com/api/matkul/view/id/1)

```json
{
  "id": 1,
  "kode_matkul": "CSIE604274",
  "nama_matkul": "Administrasi Sistem",
  "dosenList": [
    {
    "id": 1,
    "nip": "1290578781",
    "nama": "Heri Kurniawan S.Kom., M.Kom."
    }
  ]
}
```

## api/matkul/view/kode/[kode_matkul]

Mengembalikan object sebuah mata kuliah dengan menggunakan kode mata kuliah

**URL** : `/api/matkul/view/kode/[kode_matkul]`

**Method** : `GET`

### Response

**Contoh Request**: [/api/matkul/view/kode/CSIE604274](https://apap-fasilkom.herokuapp.com/api/matkul/view/kode/CSIE604274)

```json
{
  "id": 1,
  "kode_matkul": "CSIE604274",
  "nama_matkul": "Administrasi Sistem",
  "dosenList": [
    {
    "id": 1,
    "nip": "1290578781",
    "nama": "Heri Kurniawan S.Kom., M.Kom."
    }
  ]
}
```

## api/dosen/viewAll

Mengembalikan daftar seluruh dosen

**URL** : `/api/dosen/viewall`

**Method** : `GET`

### Response

**Contoh Request**: [/api/dosen/viewall](https://apap-fasilkom.herokuapp.com/api/dosen/viewall)

```json
[
  {
    "id": 15,
    "nip": "1290578809",
    "nama": "Puspa Indahati Sandhyaduhita S.T., M.Sc.",
    "mataKuliahList": [
      {
        "id": 13,
        "kode_matkul": "CSIE604165",
        "nama_matkul": "Manajemen Rantai Suplai"
      },
      {
        "id": 18,
        "kode_matkul": "CSIM603229",
        "nama_matkul": "Proyek Pengembangan Sistem Informasi"
      }
    ]
  },
  {
    "id": 12,
    "nip": "1290578803",
    "nama": "Qorib Munajat S.Kom.,M.I.S.",
    "mataKuliahList": [
      {
        "id": 11,
        "kode_matkul": "CSIE604378",
        "nama_matkul": "Manajemen Layanan TI"
      }
    ]
  },
]
```

## api/dosen/view/id/[id_dosen]

Mengembalikan object seorang dosen dengan menggunakan ID dosen

**URL** : `/api/dosen/view/id/[id_dosen]`

**Method** : `GET`

### Response
**Contoh Request**: [/api/dosen/view/id/1](https://apap-fasilkom.herokuapp.com/api/dosen/view/id/1)

```json
{
  "id": 1,
  "nip": "1290578781",
  "nama": "Heri Kurniawan S.Kom., M.Kom.",
  "mataKuliahList": [
    {
      "id": 1,
      "kode_matkul": "CSIE604274",
      "nama_matkul": "Administrasi Sistem"
    }
  ]
}
```

## api/dosen/view/nip/[nip]

Mengembalikan object seorang dosen dengan menggunakan nip dosen

**URL** : `/api/dosen/view/nip/[nip]`

**Method** : `GET`

### Response

**Contoh Request**: [/api/dosen/view/nip/1290578781](https://apap-fasilkom.herokuapp.com/api/dosen/view/nip/1290578781)

```json
{
  "id": 1,
  "nip": "1290578781",
  "nama": "Heri Kurniawan S.Kom., M.Kom.",
  "mataKuliahList": [
    {
      "id": 1,
      "kode_matkul": "CSIE604274",
      "nama_matkul": "Administrasi Sistem"
    }
  ]
}
```

## api/staf/viewAll

Mengembalikan daftar seluruh staf

**URL** : `/api/staf/viewall`

**Method** : `GET`

### Response

**Contoh Request**: [/api/staf/viewall](https://apap-fasilkom.herokuapp.com/api/staf/viewall)

```json
[
  {
    "id": 36,
    "nip": "1506737823",
    "nama": "Wendy Damar Wisma Trisna Bayu"
  },
  {
    "id": 37,
    "nip": "1506689692",
    "nama": "Savira Nurul Ahila"
  },
  {
    "id": 38,
    "nip": "1506723231",
    "nama": "Teuku Amrullah Faisal"
  }
]
```

## api/staf/view/id/[id_staf]

Mengembalikan object seorang staf dengan menggunakan ID staf

**URL** : `/api/staf/view/id/[id_staf]`

**Method** : `GET`

### Response
**Contoh Request**: [/api/staf/view/id/36](https://apap-fasilkom.herokuapp.com/api/staf/view/id/36)

```json
{
  "id": 36,
  "nip": "1506737823",
  "nama": "Wendy Damar Wisma Trisna Bayu"
}
```

## api/staf/view/nip/[nip]

Mengembalikan object seorang staf dengan menggunakan nip staf

**URL** : `/api/staf/view/nip/[nip]`

**Method** : `GET`

### Response

**Contoh Request**: [/api/staf/view/nip/1506737823](https://apap-fasilkom.herokuapp.com/api/staf/view/nip/1506737823)

```json
{
  "id": 36,
  "nip": "1506737823",
  "nama": "Wendy Damar Wisma Trisna Bayu"
}
```
