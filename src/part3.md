## Part3. Telegram Bot

1. Open [BotFather](https://t.me/BotFather) and follow the instructions to create a new bot and get a token.
2. Set the current value of the `token` [variable](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/collection/34616296-d8511e35-bfe2-4e73-8d69-501d892e07df?tab=variables) using the bot token from [(1)](#1-open-botfather-and-follow-the-instructions-to-create-a-new-bot-and-get-a-token)
3. Check the API requests:
   
   - The bot info (method `getMe`)
  
       [<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/request/34616296-24742a74-40bb-46ca-9303-fec51d8ab83b)

   - Method `getUpdates` to get `user_id` and `chat_id`
      
       [<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/request/34616296-28effae1-38b7-44fe-8dda-f2e102d16f10)

4. After this you need to set the current value of the `chat_id` [variable](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/collection/34616296-d8511e35-bfe2-4e73-8d69-501d892e07df?tab=variables) using the `chat_id` from the response of the `getUpdates` request.
5. Check the rest of API requests:
  
   - Send message with `sendMessage`
      
       [<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/request/34616296-79325dfc-22d9-4c12-b0c7-821a5e9c93cc)

   - Send a photo from the bot
      
       [<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/request/34616296-c07b02ea-167e-44e1-a03b-10e44bbbf2d7)

   - Send `pdf` with the same method `sendPhoto`
      
       [<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/request/34616296-265204a5-9ee9-4a20-a682-f042d9d5e148)

   - Send `docx` instead of `pdf`
      
       [<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/request/34616296-aef008d4-0b7a-459b-9034-46cf8136189b)

   - Get user profile photos with `getUserProfilePhotos`
      
       [<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" style="width: 128px; height: 32px;">](https://www.postman.com/security-explorer-76171055/workspace/scp-elidacon-backend-project1/request/34616296-d4fe47e0-0838-4081-ba6c-f29a4429aed8)

