function step1Switch(e){
    document.querySelector('.step1 .start').classList.add('next');
}

function moveTop(){
    event.stopPropagation();
    document.querySelector('.step1').classList.add('goTop');
}

document.querySelector('.step2 .delete').addEventListener('click', (e)=>{
    document.querySelector('.step1').classList.remove('goTop');
});

document.querySelector('#fidelity_login').addEventListener('click', (e)=>{
    document.querySelector('.fidelity-email').classList.add('show');
});

document.querySelector('#sign_fidelity').addEventListener('click', (e)=>{
    document.querySelector('.step3').classList.add('show');
});

document.querySelector('#google_login').addEventListener('click', (e)=>{
    document.querySelector('.google').classList.add('show');
});

document.querySelector('#toStep3').addEventListener('click', (e)=>{
    document.querySelector('.step3').classList.add('show');
});

document.querySelector('#toStep4').addEventListener('click', (e)=>{
    document.querySelector('.step4').classList.add('show');
});

document.querySelectorAll('.move-button').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        document.querySelector('.step5').classList.add('show');
    });
});


document.querySelector('#toStep6').addEventListener('click', (e)=>{
    document.querySelector('.step6').classList.add('show');
});

document.querySelector('#clearPre').addEventListener('click', (e)=>{
    document.querySelector('.pre-login').classList.add('done');
});



//--------------------------------Home------------------------------------
document.querySelector('.menu-trigger').addEventListener('click', (e)=>{
    e.target.classList.toggle('expand');
});


document.querySelector('.add.button').addEventListener('click', (e)=>{
    e.target.classList.toggle('show-options');
});

document.querySelector('#goPayment').addEventListener('click', (e)=>{
    document.querySelector('.custody.payment').classList.add('show');
    document.querySelector('.add.button').click();
});

document.querySelector('#goSwap').addEventListener('click', (e)=>{
    document.querySelector('.custody.swap').classList.add('show');
    document.querySelector('.add.button').click();
});


//--------------------------------Payment------------------------------------
document.querySelectorAll('.contract').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        document.querySelector('#contractInput').value = item.querySelector('span:last-child').innerText;
    });
});

document.querySelector('#contractPaste').addEventListener('click', (e)=>{
    document.querySelector('.payment .top-bar').classList.toggle('backable');
    e.target.style.display = 'none';
    document.querySelectorAll('.contract-list, .coin-list').forEach((item)=>{
        item.classList.toggle('show');
    });
});

document.querySelectorAll('.coin').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        document.querySelector('.transfer-info').classList.add('show');
        document.querySelector('.coin-list').classList.remove('show');
        document.querySelector('.payment .bottom-button-container').removeAttribute('hidden');
    });
});


// keyboard
let payValue= [];

document.querySelectorAll('.payment .num-board .key').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        if(e.target.innerText){
            if(e.target.innerText === '.' && payValue.indexOf('.')<0){
                payValue.push('.');
            } else if(e.target.innerText!=='.'){
                payValue.push(e.target.innerText);
            }
        } else {
            payValue.pop();
        }

        document.querySelector('.dis-val').innerText = payValue.toString().replaceAll(',','');
    });
});


document.querySelector('#goToTransferDetail').addEventListener('click', (e)=>{
    e.target.classList.remove('show');
    e.target.closest('.step').nextElementSibling.classList.toggle('show');
});

document.querySelector('#payConfirm').addEventListener('click', (e)=>{
    e.target.classList.remove('show');
    e.target.closest('.step').nextElementSibling.classList.toggle('show');

    e.target.closest('.payment').querySelector('.top-bar').classList.add('hidden');
});


//--------------------------------swap------------------------------------

document.querySelector('.swap-list').addEventListener('click', (e)=>{
    document.querySelector('.custody.swap .screen').classList.toggle('show');
    document.querySelector('.custody.swap .swap-list').classList.toggle('show');
})

let fromToIndicator = '';

document.querySelectorAll('.swap-container>div').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        fromToIndicator = e.target.classList.contains('from')? 'from': 'to';
        document.querySelector('.swap-list').click();
    })
});

document.querySelectorAll('.swap-coin').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        const coin = e.target.closest('.swap-coin');

        if(!coin.classList.contains('selected')){
            coin.classList.add('selected')
            let swapItem = document.querySelector(`.swap-container>.${fromToIndicator}`);
            swapItem.classList.remove('empty');
            swapItem.innerHTML = '';
            swapItem.append(coin.querySelector('img').cloneNode());
            swapItem.append(coin.querySelector('h4').cloneNode(true));

            if(document.querySelectorAll('.swap-container .empty').length === 0){
                document.querySelector('.swap .transfer-val').classList.add('show');
                document.querySelector('.swap .num-board').classList.add('show');
                document.querySelector('.swap .step1 .bottom-button-container').classList.add('hideCopy');
            } else {
                document.querySelector('.swap .transfer-val').classList.remove('show');
                document.querySelector('.swap .num-board').classList.remove('show');
            }
        }
    });
});

// keyboard
let swapValue= [];

document.querySelectorAll('.swap .num-board .key').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        if(e.target.innerText){
            if(e.target.innerText === '.' && swapValue.indexOf('.')<0){
                swapValue.push('.');
            } else if(e.target.innerText!=='.'){
                swapValue.push(e.target.innerText);
            }
        } else {
            swapValue.pop();
        }

        document.querySelector('.transfer-val .val').innerText = swapValue.toString().replaceAll(',','');
        document.querySelector('.swap .step1 .bottom-button-container').classList.add('continue');
    });
});

document.querySelectorAll('#swapReview, #swapConfirm').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        e.target.classList.remove('show');
        e.target.closest('.step').nextElementSibling.classList.toggle('show');
    });
});

document.querySelectorAll('#swapDone, #payDone').forEach((item)=>{
    item.addEventListener('click', (e)=>{
        const branch = e.target.closest('.custody');
        branch.classList.remove('show');

        setTimeout(()=>{
            branch.querySelectorAll('.step').forEach((item, index)=>{
                if(index === 0){
                    item.classList.add('show');
                } else {
                    item.classList.remove('show');
                }
            });
        }, 1000);
    });
});

