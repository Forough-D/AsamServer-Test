<template>
  <div class="container mt-4">
    <Styles/>
    <div class="row invoiceStyles">
      <div class="col col-lg-8 InvoiceCard">
        <div class="InvoiceCardHeader">
          <div class="InvoiceCardTitle">
            <p class="invoiceTitle">
              Invoice #26773
            </p>
            <p class="invoicePaidStatus">
              Unpaid
            </p>
          </div>
          <div class="InvoiceContacts">
            <span class="">
              <p class="invoiceContactsTextsTitle">Invoiced To</p>
              <p class="invoiceContactsTexts">Granit Empty</p>
              <p class="invoiceContactsTexts">granit.empty@gmail.com</p>
              <p class="invoiceContactsTexts">United States</p>
              
            </span>
            <span class="invoicedToIcon">
            </span>
            <span class="">
              <p class="invoiceContactsTextsTitle">Pay To</p>
              <p class="invoiceContactsTexts">OperaVPS Ltd.</p>
              <p class="invoiceContactsTexts">47 Wharf Rd, N1 7GS</p>
              <p class="invoiceContactsTexts">London, United Kingdom</p>
            </span>
          </div>
        </div>
        <div class="paymentMethodCards">
        <div class="paymentMethods">
          <span class="paymentMethodTitle">Payment Method</span>
          <div class="paymentMethodBox">
          <div>
            <p class="pMethodCardTitle">
              <img src="../assets/img/icons/card-pos.svg" alt="">
              Apply Credit
            </p>
          </div>
          <div class="pMethodBodyDiv">
            <span>
              <p>
                The amount in your account is 
                <em class="priceColor">
                  $50.00 USD
                </em>
                .
              </p>
              <p>
                Do you want this amount to be taken off 
                <em class="thisInvoiceColor">
                  this invoice
                </em>
                ?
              </p>
              <p>
                Please type the number you want in the box below and click "
                <em class="applyColor">
                  Apply
                </em>
                ."
              </p>
            </span>
            <span class="priceInputGroup">
              <input class="priceInput" value="15.00" type="text">
              <button class="priceInputSubmitBtn">Apply</button>
            </span>
            </div>
          </div>
        </div>
        <img class="orSection" src="../assets/img/icons/GroupOr.png" alt="">
        <div class="paymentMethods">
          <div class="paymentMethodBox">
          <div>
            <span class="pMethodCryptoCardTitle">
              <span>
                <soft-radio >Crypto Currency</soft-radio>
              </span>
              <span class="pMethodCryptoTitleSpan">
                <img src="../assets/img/icons/Bitcoin.png" alt="">
                <img src="../assets/img/icons/Et.png" alt="">
                <img src="../assets/img/icons/Lightcoin.png" alt="">
                <img src="../assets/img/icons/BitcoinCash.png" alt="">
              </span>
            </span>
          </div>
          <div class="pMethodCryptoBodyDiv">
            <span class="pMethodCryptoBodyDivTexts">
              <p>
                The 
                <em class="thisInvoiceColor">
                  Crypto Currency
                </em>
                  gatway is  
                <em class="priceColor">
                  Tax-free
                </em>
                and you can use different currencies such as 
                <em class="thisInvoiceColor">
                  Bitcoin, Ethereum, Ripple, Tether
                </em>
                 and other currencies.
              </p>
              <p>
                <em class="thisInvoiceColor">
                  Crypto Currency
                </em>
                 transactions can be processed between 
                <em class="thisInvoiceColor">
                  30 minutes and 3 days
                </em>
                and please wait at least 30 minutes after payment to receive a
                <em class="thisInvoiceColor">
                  response from the blockchain
                </em>
                network
              </p>
            </span>
            <span class="cryptoPriceInputGroup">
              <p class="cryptoPriceInputSubmitBtn">Sub Total</p>
              <p class="cryptoPriceInputSubmitBtn">$40.98 USD</p>
            </span>
            <span class="cryptoDiscountInputGroup">
              <p class="cryptoDiscountInputSubmitBtn">Discount Code</p>
              <p class="cryptoDiscountInputSubmitBtn">Do you have a discount code?</p>
              <input class="discountInput" value="" type="text">
              <p class="cryptoDiscountInputBtnText">$0 USD</p>
            </span>
            <span class="cryptoPriceTotalInputGroup">
              <p class="cryptoPriceInputSubmitBtn">Total</p>
              <p class="cryptoPriceInputSubmitBtn">$40.98 USD</p>
            </span>
            <button class="PayNowBtn">PAY NOW ($157.9 USD)</button>

            </div>
          </div>
        </div>
          <div class="paymentMethodBoxIncreased">
            <span class="pMethodCardIncreasedTitle">
              <soft-radio >PayPal</soft-radio>
            </span>
            <span class="pMethodCryptoTitleSpan">
                <img src="../assets/img/icons/PayPal.png" alt="">
              </span>
        </div>
        <div class="paymentMethodBoxIncreased">
            <span class="pMethodCardIncreasedTitle">
              <soft-radio >Credit Card</soft-radio>
            </span>
            <span class="pMethodCryptoTitleSpan">
                <img src="../assets/img/icons/Stripe.png" alt="">
                <img src="../assets/img/icons/Discover.png" alt="">
              </span>
        </div>
        <div class="paymentMethodBoxIncreased">
            <span class="pMethodCardIncreasedTitle">
              <soft-radio >Web Money</soft-radio>
            </span>
            <span class="pMethodCryptoTitleSpan">
                <img src="../assets/img/icons/Webmoney.png" alt="">
              </span>
        </div>
        <div class="InvoiceItemsCard">
          <span class="invoiceItemsTitleSpan">
            <p class="invoiceItemsTitle">
              Invoice Items
            </p>
            <i class="fa fa-angle-down	"></i>
          </span>
          <span class="invoiceItemsTitleSpan">
            <p class="invoiceItemsTitle">
              <em class="invoiceItemsTitleEm">(</em> 4 <em class="invoiceItemsTitleEm">item/s included)</em>
            </p>
          </span>
        </div>
</div>
</div>
<div class="col col-lg-8 InvoiceBtnGroup">
  <button class="InvoiceBtn">Print Invoice</button>
  <Button class="InvoiceBtn">Download PDF</Button>
</div>
    </div>
  </div>
    
</template>

<script>
// import SoftButton from "@/components/SoftButton.vue";
import SoftRadio from "@/components/SoftRadio.vue";

export default {
  name: "Billing",
  components: {
    // SoftButton,
    SoftRadio,
  },
};
</script>
<style scoped>
 .invoiceStyles {
  justify-content: center;
  padding: 15px;
 }
 .InvoiceCard {
  padding: 20px 20px;
  border: 2px solid #edeff1;
  border-radius: 5px;
 }
 .InvoiceCardHeader {
  padding: 20px;
 }
 .InvoiceCardTitle {
  display: flex;
  justify-content: space-between;
 }
 .invoicePaidStatus {
  background-image: url("../assets/img/icons/Group7049.png");
  background-repeat: no-repeat;
    width: 106px;
    display: flex;
    font-size: 14px;
    color: #ff6b6b;
    justify-content: center;
    align-items: center;
    padding: 0;
    margin: 0;
    height: 35px;
    padding-left: 15px;
    margin-right: -40px;
   }
 .invoiceTitle {
  font-size: 30px;
  color: #000;
 }
 .InvoiceContacts {
  display: flex;
  justify-content: space-between;
  margin-top: 30px;
 }
 .invoiceContactsTextsTitle {
  font-size: 15px;
  font-weight: bold;
 }
 .invoiceContactsTexts {
  font-size: 13px;
  padding: 0px;
  line-height: 0.3;
 }
 .invoicedToIcon {
  background-image: url("../assets/img/icons/invoice-back.png");
  background-repeat: no-repeat;
  width: 33%;
 }
 .paymentMethodCards {
  display: flex;
  flex-direction: column;
  gap: 15px;
 }
 .paymentMethods {
  display: flex;
  flex-direction: column;
  gap: 5px;
 }
 .paymentMethodTitle {
  font-size: 15px;
  font-weight: bold;
  padding: 20px;
 }
 .paymentMethodBox {
  border: 1px solid #2bab89;
  border-radius: 4px;
 }
 .pMethodCardTitle {
  color: #2bab89;
  padding: 10px;
  border-bottom: 1px solid #2bab89;  
 }
 .pMethodCryptoCardTitle {
  display: flex;
  justify-content: space-between;
  color: #2bab89;
  padding: 10px;
  border-bottom: 1px solid #2bab89;  
 }
 .pMethodCryptoTitleSpan {
  display: flex;
  align-items: center;
  gap: 8px;
 }
 .pMethodCardTitle>img {
  margin-right: 10px;
 }
 .pMethodBodyDiv {
  display: flex;
  flex-direction: row;
  align-items: center;
    justify-content: space-between;
  padding: 0px 0px 0px 15px;
    border-left: 2px solid #EDEFF1;
    margin: 35px 35px 30px 20px;
    font-size: 14px;
 }
 .pMethodCryptoBodyDiv {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin: 35px 35px 30px 20px;
    font-size: 14px;
    gap: 8px;
 }
.pMethodCryptoBodyDivTexts {
  border-left: 2px solid #EDEFF1;
  padding: 0px 0px 0px 15px;
  margin-bottom: 40px;

}
 .pMethodBodyDiv>p {
  font-size: 14px;
  margin-bottom: 6px;
 }
 .applyColor {
  color: #2bab89;
 }
 .thisInvoiceColor {
  font-weight: bold;
 }
 .priceColor {
  color: #2bab89;
 }
 .priceInputGroup
 {
  display: flex;
  flex-direction: row;
  align-items: center;
 }
 .cryptoPriceInputGroup {
  display: flex;
  justify-content: space-between;
  border: 1px solid #EDEFF1;
  font-size: 10px;
  padding: 8px 15px;
  border-radius: 4px;
  font-weight: bold;
  color: #000;
 }
 .cryptoDiscountInputGroup {
  display: flex;
  color: #000;
  border: 1px solid #EDEFF1;
  font-size: 10px;
  border-radius: 4px;
  font-weight: bold;

 }
 .cryptoPriceTotalInputGroup {
  display: flex;
  justify-content: space-between;
  background: #EDEFF1;
  color: #000;
  font-size: 10px;
  padding: 8px 15px;
  border-radius: 4px;
  font-weight: bold;
 }
 .cryptoPriceInputSubmitBtn {
  margin: 0;
  font-size: 14px;
  border-radius: 4px;
 }
 .cryptoDiscountInputSubmitBtn {
  border-left: 1px solid #EDEFF1;
  margin: 0;
  padding: 10px 15px;
  font-size: 14px;
  border-radius: 4px;
  min-width: max-content;
 }
 .cryptoDiscountInputBtnText {
  margin: 0;
  padding: 10px 15px;
  font-size: 14px;
  border-radius: 4px;
  min-width: max-content;
 }
 .priceInput {
  border: 1px solid #EDEFF1;
  height: 45px;
  padding: 10px;
  border-radius: 4px;
  width: 140px;
  color: #000;
 }
.discountInput {
  background: #f8f9fa;
  border: none;
  border-left: 1px solid #EDEFF1;
  width: 100%;
  height: auto;
  padding: 10px;
 }
 .input.form-check-input {
  background: #2bab89 !important;
 }
 .priceInputSubmitBtn {
  background: #E9F7F3;
  color: #2bab89;
  border: none;
  padding: 0px 10px;
  margin-left: -62px;
  height: 35px;
  border-radius: 4px;
 }
 .orSection { 
  width: 100%;
  height: 30px;
  object-fit: contain;
 }
 .form-check-input:checked[type=radio] {
    background-image: linear-gradient(310deg, #66d432 0%, #66d432 100%) !important;
}
.paymentMethodBoxIncreased {
  display: flex;
  justify-content: space-between;
  border-radius: 4px;
  border: 1px solid #2bab89;
  padding: 10px;
}
.pMethodCardIncreasedTitle {
  margin: 0;
}
.InvoiceItemsCard {
  display: flex;
  flex-direction: row;
  align-items: center;
  padding: 15px 30px;
  background: #EDEFF1;
  border-radius: 4px;
  justify-content: space-between;
}
.invoiceItemsTitle {
  margin: 0;
    font-size: 14px;
    font-weight: bold;
    margin-right: 20px;
}
.invoiceItemsTitleSpan {
  display: flex;
  align-items: center;
}
.invoiceItemsTitleEm {
  font-weight: 400;
}
.InvoiceBtnGroup {
  padding: 20px 0px;
    display: flex;
    justify-content: flex-end;
    gap: 10px;
}
.InvoiceBtn {
  padding: 6px 12px;
  border: none ;
    background: #EDEFF1;
    color: #000;
    border-radius: 4px;
}
.PayNowBtn {
  padding: 12px;
  border: none ;
    background: #2bab89;
    color: #fff;
    border-radius: 4px;
}
 </style>