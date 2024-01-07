//MODEL STUDIO

# include <iostream>
# include <stream>
#include "..../Database/Databasestudio.h"
using namespace std;

void mAddStudio(String inputnamastudio,int inputjumlahkursi){
    namastudio(nstudio) = inputnamastudio;
    jumlahkusi(nstudio) = inputjumlahkursi;
    nstudio++;
}

void mviewstudio(){
    count &lt;&lt; &quot;Daftar studio&quot;&lt;&lt;endl;
    for (int i=0 ; i &lt; nstudio;i++){
        count <<"nama studio:"<<namastudio[i]<<endl;
        count <<"jumlah kursi" << jumlahkursi[i]<<endl;
        cout endl;
    }
}
int msearchstudio(string inoutnamastudio) {
    int index= -i ;
    for (int i= 0;i&lt;nstudio;i++) {
        if (namastudio(i)) ==inoutnamastudio {
                index = -1;
                break;
        }
    }
    return indext;
}

//MODEL FILM

#include <string>
#include <iostream>
#include ".../Database/Databasefilm.h"
using namespace std;

void mAddfilm (string inputjudulfilm,string inputgenrefilm,string inputdurasifilm) {
    judulfilm [nfilm]=inputjudulfilm;
    genrefilm [nfilm]=inputgenrefilm;
    durasifilm [nfilm]=inputdurasifilm;
    nfilm;
}

void mviewfilm (){
    count <<"daftar film",<<endl;
    for (int i=0;i <nfilm:i++) {
        cout<<"judul film:" <<judulfilm[i]<<endl;
        cout<<"genre film:" <<genrefilm[i]<<endl;
        cout<<"durasi film:" <<durasifilm[i]<<endl;
        count <<endl;
    }
}

int msearchfilm (string inputjudulfilm) {
    int index=-1;
    for(int i=0;i < nfilm; i++){
        if (judulfilm [i] == inputjudulfilm) {
            index =i;
            break;
        }
    }
    return index;
}

//VIEW STUDIO

# include <iostream>
# include <string>
# include ".../Model/Modelstudio.h"
using namespacestd ;

void .addstudio () {
    string namastudioinput;
    int jumlahkursiinput;
    cout<<"masukan nama studio:";
    cin>>nama studio input;
    cout<<"masukan jumlah kursi:";
    cin>> jumlahkursiinput
    m Addstudio (inputnamastudio:namastudioinput,jumlahkursiinput:jumlahkursiinput);
}

void viewstudio(){
    mviewstudios();
}

void vsearchstudio() {
    string namastudioinput;
    cout<<"masukan nama studio:";
    cin>>namastudioinput;
    int index = mSearchstudio(inputnamastudio:namastudioinput);
    if (index !=-1) {
        cout<<"nama studio:" << namastudio(index)<<endl;
        cout<<"jumlah kursi:" << jumlahkursi(index)<<endl;
    }else{
        cout<<"studio tidak ditemukan"<<endl;
    }
}


//VIEW FILM

#include <iostream>
#include <string>
#include ".../model/modelfilm.h"

using namespace std;

void Vaddfilm (){
    string judulfilminput;
    string genrefilminput;
    string durasifilminput;
    cout<<"masukan judul film: ";
    cin >>judulfilminput;
    cout<<"masukan genre film: ";
    cin>>genrefilminput;
    cout<<"masukan durasi film: ";
    cin>>durasifilminput;
    maddfilm(inputjudulfilm: judulfilminput, inputgenrefilm:genrefilminput,inputdurasifilm:durasifilminput);
}

void vviewfilms (){
    mviewfilms();
}

void vsearchfilmfilm(){
    string judulfilminput;
    cout <<"masukan judul film:";
    cin>>judulfilminput;
    int index= msearchfilm(inputjudulfilm: judulfilminput);
    if (index !:-1) {
        cout<<"masukan judul film: " <<judulfilm [index] <<endln;
        cout<<"masukan genre film: " <<genrefilm [index] <<endln;
        cout<<"masukan durasi film: " <<durasifilm [index] <<endln;
    }else{
        cout <<"file tidak di temukan" <<endl ;
    }
}

//MODEL JADWAL

#include "..../database/databasejadwal"
#include <iostream>
#include <string>
using namespace std;

void mjadwal (string inputjamtayang,string inputtanggaltayang,string inputnamastudio,string inputfilm,string inputhargatiket) {
    int indexstudio = msearchstudio(inpnamastudiotayang);
    int indexfilm = msearchfilm(inpjudulfilmtayang);
    if (indexstudio != -1 && indexfilm != -1) {
        kodetayang[njadwal] = njadwal + 1;
        jamtayang[njadwal] = inpjamtayang;
        tanggaltayang[njadwal] = inptanggaltayang;
        namastudiotayang[njadwal] = inpstudiotayang;
        judulfilmtayang[njadwal] = inpjudulfilm;
        hargatiket[njadwal] = inphargatiket;
        njadwal++;
    } else{
        cout <<"studio atau film tidak ditemukan<<endl";
    }
}

void mviewjadwal(){
    cout<<"daftar jadwal"<<endl;
    for (inti=o;1 <njadwal;1++){
        cout<<"kode tayang"<<kodetayang[1]<<endl;
        cout<<"jamtayang"<<jamtayang[1]<<endl;
        cout<<"tanggaltayang"<<tanggaltayang[1]<<endl;
        cout<<"nama studio"<<namastudiotayang[1]<<endl;
        cout<<"judul film"<<judulfilmttayang[1]<<endl;
        cout<<"harga tiket"<<hargatiket[1]<<endl;
        cout<<endl;
    }
}
int msearchjadwal(int inpkodetayang) {
    int index = -1;
    for (inti = 0; i < njadwal; i++) {
        if (kode tayang[i]==inpodetayang){
            index = -1;
            break;
        }
    }
    return index;
}


//VIEW JADWAL

#include ".../model/modeljadwal.h"
#include <iostream>
#include <string>
using namespace std;

void vaddjadwal(){
    string jamtayanginput;
    string tanggaltayanginput;
    string namastudiotayanginput;
    string judulfilmtayanginput;
    int hargatiket;
    cout <<"masukan jam tayang:";
    cin >>jamtayanginput;
    cout <<"masukan tanggal tayang:";
    getline (&: cin,&:tanggaltayanginput);
    cout <<"masukan nama studio tayang:";
    getline (&:cin,&:namastudiotayanginput);
    cout <<"masukanjudulfilmtayang:";
    getline(&:cin,&:judulfilmtayanginput);
    cout <<"harga tiket:";
    cin >>hargatiketinput;
    maddjadwal(inpjamtayang:jamtayanginput,inptanggaltayang:tanggaltayanginput,inpnamastudiotayang:namastudiotayang,inpjudulfilmtayang:judulfilmtayanginput,inphargatiket:hargatiketinput);
}

void vviewjadwals(){
    mviewjadwal;
}
void vsearchjadwal(){
    int kodetayanginput;
    cin >>kodetayanginput;
    int index=msearchjawal(inpkodetayang:kodetayanginput);
    if (index !=-1){
        cout <<"kodetayang:"<<kodetayang[index]endl;
        cout <<"jamtayang:"<<jamtayang[index]endl;
        cout <<"tanggaltayang:"<<tanggaltayang[index]endl;
        cout <<"namastudio:"<<namastudio[index]endl;
        cout <<"judulfilm:"<<judulfilm[index]endl;
        cout <<"hargatiket:"<<hargatiket[index]endl;
    } else{
        cout<<"jadwal tidak ditemukan"<<endl;
    }
}

