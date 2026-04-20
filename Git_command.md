## Git Tüm Komutları 



git config --global user.name "\[isim]"            Git kayıtlarında (commit) görünecek yazar ismini ayarlar.

git config --global user.email "\[email]"	  Git kayıtlarında görünecek e-posta adresini ayarlar.

git init                                          Bulunduğun klasörü boş bir Git deposu (repository) haline getirir ve izlemeye başlar.

git clone \[url]                                   GitHub, GitLab vb. bir yerdeki projeyi tüm geçmişiyle bilgisayarına indirir.

git status                                        Hangi dosyaların değiştiğini, yeni eklendiğini veya silindiğini özet halinde gösterir.

git add \[dosya]                                   Belirli bir dosyadaki değişiklikleri "sahneye" (staging area) alır. Kaydetmeye hazırlar.

git add .                                         Klasördeki tüm değişiklikleri (yeni, değişen, silinen) tek seferde sahneye alır.

git commit -m "\[mesaj]"                           Sahnedeki değişiklikleri bir paket haline getirir ve belirlediğin mesajla kalıcı olarak kaydeder.

git rm \[dosya]                                    Bir dosyayı hem bilgisayardan siler hem de bu silme işlemini Git'e bildirir.

git remote add origin \[url]                       Yerel deponu, uzak bir sunucudaki depoya bağlar. (Az önce terminalinde yazdığımız komut).

git push -u origin master                         Yereldeki commit'lerini uzak sunucuya (örn: GitHub'daki master dalına) yükler

git pull                                          Uzak sunucuda başkasının yaptığı değişiklikleri senin bilgisayarına çeker ve kodunla birleştirir

git fetch                                         Uzak sunucudaki değişiklikleri bilgisayarına sadece indirir ancak senin kodlarınla otomatik birleştirmez (Güvenli kontrol).

git branch                                        Projedeki mevcut dalları listeler ve şu an hangisinde olduğunu gösterir (\* ile).

git branch \[dal\_adi]                              \[dal\_adi] isminde yeni bir çalışma alanı (dal) oluşturur.

git checkout \[dal\_adi]                            Belirtilen dala geçiş yapar (Git'in daha yeni sürümlerinde bunun yerine git switch \[dal\_adi] de kullanılır).

git checkout -b \[dal\_adi]                         Hem yeni bir dal oluşturur hem de anında o dala geçiş yapar (Hızlı kısayol).

git merge \[dal\_adi]                               Belirtilen daldaki kodları, şu an bulunduğun dalın içine katarak birleştirir.

git log                                           Projenin başından beri yapılan tüm commit'leri (kimin, ne zaman yaptığını) listeler. Çıkmak için q tuşuna basılır. 

git log --oneline                                 Geçmişi çok daha sade, tek satırlık özetler halinde gösterir.

git diff                                          Henüz add komutu ile sahneye almadığın satır bazlı farklılıkları (neleri sildin, neleri ekledin) yeşil ve kırmızı renklerle gösterir

git reset \[dosya]                                 Yanlışlıkla git add ile sahneye aldığın dosyayı sahneden çıkarır. (Kodlarına dokunmaz, sadece kaydetme sırasından çıkarır).

git checkout -- \[dosya]                           add yapılmamış bir dosyadaki tüm değişiklikleri iptal eder ve onu son commit'teki orijinal haline döndürür

git revert \[commit\_id]                            Eski bir commit'in yaptıklarını tam tersine çeviren (geri alan) yeni bir güvenli commit oluşturur. Geçmişi silmez.

git reset --hard                                  Son commit'ten bu yana yaptığın tüm değişiklikleri kalıcı olarak çöpe atar. Geri dönüşü yoktur, çok dikkatli kullanılmalıdır.

